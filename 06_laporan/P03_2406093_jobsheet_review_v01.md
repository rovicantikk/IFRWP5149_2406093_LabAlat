NO      Temuan                  Perbaikan yang diperlukan     Alasan
1   Aktor mahasiswa berada      Pindahkan aktor keluar      Aktor merupakan pihak eksternal
    didalam sistem              batas sistem

2   Lihat jadwal kuliah         Ubah kotak menjadi oval     Usecase harus menggunakan notasi oval
    sebagai kotak biasa

3   Aktor mahasiswa terhubung   Hubungkan mahasiswa dengan  Mahasiswa hanya bisa melihat jadwal
    dengan kelola jadwal        lihat jadwal kuliah         karena yang mengelola jadwal adalah admin

4   Identitas sistem sebagai    Ganti judul menjadI         Judul diagram harus sesuai
    sistem laboratorium         Sistem Informasi Akademik 
                                (SIA)

5   Relasi validasi KRS belum   Tambahkan relasi SIA-UC03   Validasi KRS selalu dilakukan
    ditampilkan dengan tepat    «include» SIA-UC04          dalam proses pengajuan KRS.

6   Relasi unduh bukti penga-   Tambahkan relasi SIA-UC05   Unduh bukti merupakan proses
    juan belum sesuai kondisi   «extend» SIA-UC03           opsional setelah pengajuan KRS berhasil.