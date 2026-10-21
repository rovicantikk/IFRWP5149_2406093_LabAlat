Langkah 1. Catat kebutuhan dan batas

    ID                                               Kebutuhan
SIA-R07                     Mahasiswa dan Dosen, sebagai Civitas Akademika, dapat melihat kalender akademik.
SIA-R08                     Dosen dapat menginput nilai mata kuliah yang diampunya.
SIA-R09                     Mahasiswa dapat melihat KHS untuk semester yang nilainya sudah dipublikasikan.
SIA-R10                     Admin Akademik dapat mengelola data mahasiswa.
SIA-R11                     Pengelolaan data mahasiswa terdiri dari tiga bentuk khusus: tambah, ubah, dan hapus data mahasiswa.
SIA-R12                     Model menunjukkan collaboration yang merealisasikan Input Nilai Mata Kuliah dan Lihat KHS.


langkah 2.  Identifikasi aktor dan use case

ID                  Nama use case                           Peran dalam model                               Sumber kebutuhan
SIA-UC08        Input Nilai Mata Kuliah         Use case umum; dapat dilakukan oleh Mahasiswa dan               SIA-R08
                                                Dosen sebagai Civitas Akademika            
SIA-UC09        Lihat KHS                       Use case umum; fungsi Dosen untuk menginput                     SIA-R08   
                                                nilai mata kuliah yang diampunya            
SIA-UC10        Kelola Data Mahasiswa           Use case umum; fungsi Admin Akademik dan use case               SIA-R10
                                                induk dari SIA-UC11, SIA-UC12, dan SIA-UC13                                         
SIA-UC11        Tambah Data Mahasiswa           Use case khusus dari SIA-UC10; fungsi untuk menambahkan         SIA-R11
                                                data mahasiswa                    
SIA-UC12        Ubah Data Mahasiswa             Use case khusus dari SIA-UC10; fungsi untuk mengubah            SIA-R11
                                                data mahasiswa                 
SIA-UC13        Hapus Data Mahasiswa            Use Case Khusus dari SIA-UC10; fungsi untuk menghapus           SIA-R11
                                                data mahasiswa
