Mahasiswa mengajukan KRS dengan memilih mata kuliah. Setiap pengajuan menjalankan validasi KRS yang memeriksa kelengkapan, prasyarat mata kuliah, dan benturan jadwal. Jika validasi berhasil, sistem menyimpan pengajuan berstatus menunggu persetujuan dosen wali. Pada konfirmasi penyimpanan, mahasiswa dapat memilih mengunduh bukti pengajuan. Dosen wali menyetujui atau menolak KRS dan memberikan catatan keputusan.


    ID              Kebutuhan tugas
SIA-R01         Mahasiswa dapat melihat jadwal kuliah
SIA-R02         Admin akademik dapat mengelola jadwal kuliah
SIA-R03         Mahasiswa dapat mengajukan KRS
SIA-R04         Sistem memvalidasi KRS sebagai bagian pengajuan
SIA-R05         Mahasiswa dapat mengunduh bukti jika memilihnya pada konfirmasi pengajuan
SIA-R06         Dosen wali dapat memproses persetujuan atau penolakan KRS

Batas dan asumsi:
• Pengguna telah terautentikasi.
• Data mata kuliah, prasyarat, dan jadwal tersedia.
• Validasi gagal menyebabkan pengajuan belum berhasil tersimpan.
• Unduh bukti tidak menjadi syarat keberhasilan pengajuan.
• KRS tersimpan belum berarti disetujui.
• Pembayaran, pengisian nilai, dan implementasi basis data berada di luar tugas.


   Aktor                       Tujuan terhadap sistem
Mahasiswa                   Melihat jadwal kuliah, mengajukan KRS dan mengunduh bukti pengajuan
Admin Akademik              Mengelola jadwal kuliah
Dosen Wali                  Dapat memproses persetujuan serta penolakan KRS

 
ID                  Nama use case                       Peran dalam model
SIA-UC01        Lihat jadwal kuliah                 Fungsi utama mahasiswa
SIA-UC02        Kelola jadwal kuliah                Fungsi utama admin akademik
SIA-UC03        Ajukan KRS                          Fungsi utama mahasiswa
SIA-UC04        Validasi KRS                        Perilaku yang disertakan UC03
SIA-UC05        Cetak bukti pengajuan KRS           Tambahan bersyarat pada UC03
SIA-UC06        Proses keputusan KRS                Fungsi utama dosen wali



SIA-UC03 «include» SIA-UC04
Alasan : validasi kelengkapan, prsasyarat mata kuliah, dan benturan jadwal selalu dilakukan saat pengajuan KRS


SIA-UC05 «extend» SIA-UC03
Extension Point: Konfirmasi pengajuan
Kondisi: Mahasiswa memilih unduh
Alasan : Pengajuan tetap berhasil meskipun mahasiswa tidak mengunduh bukti