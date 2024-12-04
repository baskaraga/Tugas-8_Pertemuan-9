# Tugas-8_Pertemuan-9
1. Melihat Data Mahasiswa (Read)
![image](https://github.com/user-attachments/assets/4593d383-77c1-476c-9929-af58638d60f4)
Pada halaman utama aplikasi, data mahasiswa ditampilkan menggunakan komponen ion-card, yang diisi dengan data dari API PHP (tampil.php). API ini mengembalikan seluruh data dari tabel mahasiswa. Setiap kartu memuat informasi berupa nama dan jurusan mahasiswa, serta dilengkapi tiga tombol aksi berikut:

- Edit: Membuka modal untuk mengubah data mahasiswa, mengarahkan ke proses pembaruan data.
- Hapus: Menampilkan dialog konfirmasi untuk menghapus data mahasiswa. Jika disetujui, data akan dihapus dari database.
- Tambah Mahasiswa: Tombol ini terletak di bagian bawah halaman dan memungkinkan pengguna untuk menambahkan data mahasiswa baru ke dalam database.

2. Menambah Data Mahasiswa (Create)
  ![image](https://github.com/user-attachments/assets/a23f29bd-c35e-416f-a0d3-c5b96eb83cf3)
Modal untuk menambahkan mahasiswa baru memungkinkan pengguna untuk mengisi kolom Nama Mahasiswa dan Jurusan, kemudian menekan tombol Tambah Mahasiswa. Data yang dimasukkan akan dikirim ke API PHP (tambah.php) untuk disimpan di database. Setelah proses berhasil, mahasiswa baru akan tampil di dalam daftar.

4. Mengedit Data Mahasiswa (Update)
  ![image](https://github.com/user-attachments/assets/741c6846-e4ef-43bb-ab80-d2dd33e1e9d7)
Modal Edit Mahasiswa memungkinkan pengguna untuk memperbarui informasi mahasiswa yang dipilih. Setelah perubahan dilakukan, data akan dikirim ke API PHP (edit.php) untuk memperbarui database berdasarkan ID mahasiswa. Daftar mahasiswa kemudian akan menampilkan informasi terbaru setelah proses pengeditan berhasil.

5. Menghapus Data Mahasiswa (Delete)
   ![image](https://github.com/user-attachments/assets/ad80e2b8-98fa-422e-a0bb-15d2298c2fac)
Pada daftar mahasiswa, pengguna dapat menekan tombol Hapus di samping data mahasiswa yang ingin dihapus. Sistem kemudian akan menampilkan konfirmasi untuk memastikan bahwa pengguna benar-benar ingin menghapus data tersebut. Setelah dikonfirmasi, data mahasiswa akan dihapus melalui API PHP (hapus.php) berdasarkan ID mahasiswa.
