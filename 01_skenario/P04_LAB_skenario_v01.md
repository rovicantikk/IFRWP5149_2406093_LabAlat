Skenario berikut merupakan bahan latihan yang ditetapkan untuk jobsheet, bukan hasil pengumpulan kebutuhan laboratorium nyata. Skenario ini melanjutkan potongan model Pertemuan 3.Selain mahasiswa, dosen juga meminjam peralatan laboratorium untuk kegiatan praktikum dan penelitian. Mahasiswa dan dosen sama-sama dapat melihat ketersediaan peralatan dan mengajukan peminjaman. Petugas laboratorium mengelola data peralatan: menambah peralatan baru, mengubah data peralatan, dan menghapus data peralatan yang tidak lagi dipakai. Setelah peminjaman disetujui dan alat diambil, petugas mencatat pengembalian peralatan. Pada saat mencatat pengembalian, petugas memeriksa dan mencatat kondisi peralatan. Dua use case utama pada potongan model ini, Ajukan Peminjaman dan Catat Pengembalian Peralatan, ditunjukkan realisasinya oleh collaboration yang bersesuaian. Seluruh fungsi Pertemuan 3 tetap berlaku dan tetap digambar: pemeriksaan ketersediaan di dalam pengajuan, pencetakan bukti pengajuan oleh mahasiswa, proses keputusan peminjaman oleh petugas, dan laporan peminjaman untuk kepala laboratorium. Diagram Pertemuan 4 adalah diagram Pertemuan 3 yang ditambah, bukan diagram baru yang menggantikannya.



• Mahasiswa adalah bentuk khusus dari Peminjam, dan Dosen adalah bentuk khusus dari Peminjam. Alasan: keduanya berbagi fungsi yang sama, yaitu melihat ketersediaan peralatan dan      mengajukan peminjaman.

• Asosiasi ke LAB-UC01 dan LAB-UC03 digambar satu kali, yaitu dari Peminjam. Jangan menggambar garis yang sama dari Mahasiswa dan dari Dosen.

• Asosiasi Mahasiswa ke LAB-UC05 Cetak Bukti Pengajuan tidak ikut dipindahkan dan tidak dihapus, karena fungsi itu khusus mahasiswa. Asosiasi ini menjadi contoh asosiasi tambahan milik aktor khusus.

• Periksa arah panah pada gambar: ujung segitiga kosong harus menempel pada Peminjam, bukan pada Mahasiswa dan bukan pada Dosen. Karena Peminjam digambar di tengah, panah Mahasiswa mengarah ke bawah dan panah Dosen mengarah ke atas; keduanya berakhir pada Peminjam.


LAB-UC08, LAB-UC09, dan LAB-UC10 adalah bentuk khusus dari LABUC02 Kelola Data Peralatan. Alasan: ketiganya adalah bentuk khusus
pengelolaan data peralatan.


    ID          Nama collaboration (sama dengan nama use case)           Use case yang direalisasikan
LAB-CO01                     Ajukan Peminjaman                           LAB-UC03: Ajukan Peminjaman
LAB-CO02                Catat Pengembalian Peralatan                     LAB-UC11: Catat Pengembalian Peralatan



Elemen                  LAB-UC11: Catat Pengembalian Peralatan
Sumber                  kebutuhan LAB-R09 dan LAB-R10
Tujuan                  Pengembalian tercatat dan status peminjaman serta kondisi peralatan terbarui
Aktor utama             Petugas Laboratorium
Pemicu                  Petugas memilih fungsi pencatatan pengembalian dan menentukan peminjaman yang akan dikembalikan Prasyarat Petugas telah 
                        terautentikasi; peminjaman terpilih berstatus Dipinjam
Pascakondisi berhasil   Pengembalian tercatat dengan tanggal kembali dan kondisi peralatan; status peminjaman menjadi Selesai
Pascakondisi gagal      Tidak ada pengembalian baru yang tercatat; status peminjaman tidak berubah
Include                 LAB-UC12: Periksa Kondisi Peralatan
Collaboration           LAB-CO02: Catat Pengembalian Peralatan
