Tugas ini berbeda dari tugas pertemuan sebelumnya. Tugas Pertemuan 2 adalah jadwal kuliah dan tugas Pertemuan 3 adalah pengajuan KRS. Tugas Pertemuan 4 adalah layanan hasil studi, dengan teknik generalization dan collaboration yang sama seperti studi kasus, tetapi diterapkan pada skenario baru tanpa contoh jawaban. Skenario tugas berikut fiktif untuk praktikum dan berbeda dari tugas Pertemuan 2 (jadwal kuliah) dan Pertemuan 3 (pengajuan KRS). Mahasiswa dan dosen sama-sama merupakan Civitas Akademika yang dapat melihat kalender akademik. Dosen menginput nilai mata kuliah yang diampunya setelah masa perkuliahan berakhir. Mahasiswa melihat Kartu Hasil Studi (KHS) untuk semester yang nilainya sudah dipublikasikan. Admin Akademik mengelola data mahasiswa: menambah data mahasiswa baru, mengubah data mahasiswa, dan menghapus data mahasiswa. Dua use case utama, Input Nilai Mata Kuliah dan Lihat KHS, ditunjukkan realisasinya oleh collaboration yang bersesuaian.


Langkah 3: Tetapkan generalization aktor

• Mahasiswa dan Dosen merupakan bentuk khusus dari Civitas Akademika. Alasan: Keduanya memiliki fungsi yang sama, yaitu melihat kalender akademik (SIA-UC07). Oleh karena itu, Civitas Akademika menjadi aktor umum, sedangkan Mahasiswa dan Dosen menjadi aktor khusus.

• Asosiasi ke SIA-UC07 Lihat Kalender Akademik digambar satu kali dari Civitas Akademika. Garis asosiasi tidak perlu digambar ulang dari Mahasiswa dan Dosen karena keduanya mewarisi fungsi dari aktor umum.

• Asosiasi Dosen ke SIA-UC08 Input Nilai Mata Kuliah dan Mahasiswa ke SIA-UC09 Lihat KHS tetap menjadi asosiasi khusus. Alasannya, input nilai hanya dilakukan oleh Dosen, sedangkan melihat KHS merupakan fungsi Mahasiswa untuk melihat hasil studi yang nilainya sudah dipublikasikan.

• Asosiasi Admin Akademik ke SIA-UC10 Kelola Data Mahasiswa tetap terpisah. Admin Akademik bertanggung jawab mengelola data mahasiswa, yang mencakup SIA-UC11 Tambah Data Mahasiswa, SIA-UC12 Ubah Data Mahasiswa, dan SIA-UC13 Hapus Data Mahasiswa sesuai SIA-R10 dan SIA-R11.

• Periksa arah panah generalisasi pada diagram. Ujung segitiga kosong harus mengarah ke Civitas Akademika sebagai aktor umum, bukan ke Mahasiswa atau Dosen. Dengan demikian, panah dari kedua aktor khusus berakhir pada Civitas Akademika.


Langkah 4: Tetapkan generalization use case

SIA-UC11 Tambah Data Mahasiswa, SIA-UC12 Ubah Data Mahasiswa, dan SIA-UC13 Hapus Data Mahasiswa merupakan bentuk khusus dari SIA-UC10 Kelola Data Mahasiswa. Alasan: Ketiganya merupakan bentuk khusus dari pengelolaan data mahasiswa sesuai kebutuhan SIA-R10 dan SIA-R11.


Langkah 5: Tetapkan collaboration

    ID              Nama collaboration (sama dengan nama use case)              Use case yang direalisasikan
SIA-CO01                    Input Nilai Mata Kuliah                             SIA-UC08: Input Nilai Mata Kuliah
SIA-CO02                           Lihat KHS                                    SIA-UC09: Lihat KHS


Langkah 6: Tulis Use Case Description Baru

    Elemen                              Deskripsi
ID dan nama                 SIA-UC08: Input Nilai Mata Kuliah
Sumber kebutuhan            SIA-R08 dan SIA-R12
Tujuan                      Nilai mata kuliah berhasil dimasukkan dan tersimpan dalam sistem.
Aktor utama                 Dosen
Pemicu                      Dosen memilih fungsi input nilai mata kuliah yang diampunya.
Prasyarat                   Dosen telah terautentikasi dan memiliki mata kuliah yang diampu.
Pascakondisi berhasil       Nilai mahasiswa berhasil disimpan dalam sistem.
Pascakondisi gagal          Nilai tidak tersimpan dan data nilai sebelumnya tidak berubah.
Collaboration               SIA-CO01: Input Nilai Mata Kuliah

