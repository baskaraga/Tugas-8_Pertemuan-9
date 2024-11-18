# Tugas-8_Pertemuan-9
Nama : Panji Bagaskara
NIM : H1D022106
Shift Baru: A

![image](https://github.com/user-attachments/assets/254215b2-2a61-40f4-ae90-5d95d9c0e759)
1. Pada komponen Angular MahasiswaPage, terdapat sebuah metode bernama getMahasiswa().

2. Ketika ngOnInit() dijalankan (saat komponen dibuka), metode ini akan mengirimkan permintaan GET ke tampil.php untuk mengambil seluruh data mahasiswa.

3. Di sisi backend, tampil.php menjalankan query SQL SELECT * FROM mahasiswa, mengambil data dari tabel mahasiswa, dan mengembalikannya dalam format JSON.

4. Komponen MahasiswaPage kemudian menerima data JSON tersebut dan menyimpannya ke dalam variabel dataMahasiswa, yang digunakan untuk menampilkan informasi mahasiswa di halaman.

![image](https://github.com/user-attachments/assets/d22d6423-9831-47f9-a4c5-08d4eb185e1f)

1. Ketika pengguna mengklik tombol Tambah Mahasiswa di halaman, modal input akan terbuka.

2. Di dalam modal, pengguna memasukkan data seperti Nama Mahasiswa dan Jurusan, lalu menekan tombol Tambah Mahasiswa.

3. Metode tambahMahasiswa() pada komponen MahasiswaPage mengambil data dari input, membuat sebuah objek, dan mengirim permintaan POST ke tambah.php dengan data tersebut.

4. Pada backend, tambah.php menerima data dalam format JSON, menjalankan query SQL INSERT untuk menambahkan data baru ke dalam database, lalu mengembalikan status berhasil atau gagal dalam format JSON.

5. Jika proses berhasil, modal input akan ditutup, metode getMahasiswa() dipanggil untuk memperbarui daftar, dan data yang baru ditambahkan akan langsung terlihat oleh pengguna.

![image](https://github.com/user-attachments/assets/c1229dc8-a134-480d-82c2-181fdbd35dfd)
1. Ketika pengguna mengklik tombol Hapus di sebelah data mahasiswa yang ingin dihapus, metode hapusMahasiswa() pada komponen MahasiswaPage akan menampilkan dialog konfirmasi menggunakan AlertController.

2. Jika pengguna memilih "Ya," proses penghapusan dilanjutkan; namun, jika memilih "Tidak," proses dibatalkan.

3. Saat pengguna memilih "Ya," metode hapusMahasiswa() mengirimkan permintaan DELETE atau GET ke hapus.php dengan mengirimkan id mahasiswa yang akan dihapus.

4. Pada sisi backend, hapus.php menjalankan query SQL DELETE untuk menghapus data mahasiswa sesuai dengan id yang diterima, lalu mengembalikan status hasil operasi tersebut.

5. Jika penghapusan berhasil, metode getMahasiswa() dipanggil kembali untuk memperbarui daftar, sehingga pengguna dapat melihat bahwa data mahasiswa yang dipilih telah dihapus dari tampilan.

   ![image](https://github.com/user-attachments/assets/de9f8d30-c82b-431f-b8e3-63c04853c625)
1. Saat pengguna mengklik tombol Edit di samping data mahasiswa yang ingin diubah, sebuah modal edit akan terbuka, menampilkan data Nama Mahasiswa dan Jurusan yang ada. Komponen kemudian memanggil metode ambilMahasiswa() untuk mengambil detail mahasiswa tersebut dari database.

2. Pengguna dapat mengubah data yang diperlukan, lalu menekan tombol Edit Mahasiswa.

3. Metode editMahasiswa() di komponen MahasiswaPage akan membuat objek dari data yang telah diperbarui dan mengirimkannya melalui permintaan PUT atau POST ke edit.php.

4. Di sisi backend, edit.php menerima data dalam format JSON, menjalankan query SQL UPDATE untuk memperbarui data mahasiswa berdasarkan id, dan mengembalikan status berhasil atau gagal.

5. Jika proses berhasil, modal akan ditutup, metode getMahasiswa() dipanggil kembali untuk menyegarkan daftar, dan data yang telah diperbarui akan terlihat di halaman.

