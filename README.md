# Bismillahirrahmanirrahim

## Janji
Saya Muhammad Naufal Arbanin dengan NIM 2310850 mengerjakan soal Tugas Praktikum 4 dalam mata kuliah Desain Pemrograman Berorientasi Objek untuk keberkahanNya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin.

## Desain / Gambar Aplikasi
![Image](https://github.com/user-attachments/assets/9410ccbf-a92e-4000-9639-debd2dbb395f)

## Penjelasan Kodingan / Program

#### Struktur Kelas Dalam Aplikasi

1. Menu (GUI Utama)

- Menampilkan form untuk input NIM, Nama, Jenis Kelamin, dan Angkatan

- Memiliki tombol Add, Delete, Cancel, Delete All

- Menampilkan tabel daftar mahasiswa

2. Mahasiswa (Model Data)

- Menyimpan atribut mahasiswa (NIM, Nama, Jenis Kelamin, Angkatan)

3. MahasiswaTableModel (Model untuk JTable)

- Mengatur bagaimana data mahasiswa ditampilkan dalam tabel

#### Penjelasan Setiap Komponen dan Alurnya
1. Form Input Mahasiswa
- Di dalam class Menu, terdapat input form yang terdiri dari:

  - NIM → JTextField nimField

  - Nama → JTextField namaField

  - Jenis Kelamin → JComboBox genderComboBox

  - Angkatan → JComboBox angkatanComboBox

- Alur Input Data
  - Pengguna mengetik NIM dan Nama di text field.

  - Pengguna memilih Jenis Kelamin dari dropdown (JComboBox).

  - Pengguna memilih Angkatan dari dropdown (JComboBox).

  - Setelah semua terisi, pengguna menekan tombol "Add" untuk menambahkan data.

2. Tombol "Add" (Menambahkan Data)
- Alur Tombol "Add"
  - Mengambil data dari form input (NIM, Nama, Jenis Kelamin, Angkatan).

  - Jika NIM atau Nama kosong, tampilkan peringatan JOptionPane.

  - Jika semua data sudah diisi, buat objek baru Mahasiswa dan tambahkan ke listMahasiswa.

  - Panggil setTable() untuk memperbarui tabel.

  - Bersihkan form input untuk input selanjutnya.

3. Tabel Mahasiswa (Menampilkan Data)
Setelah data ditambahkan, tabel akan diperbarui menggunakan MahasiswaTableModel.
- Cara Kerja Tabel
  - Menggunakan AbstractTableModel untuk menampilkan data mahasiswa dalam tabel.

  - Metode getValueAt() mengambil data dari listMahasiswa berdasarkan indeks.

  - Tabel akan diperbarui setiap kali tombol "Add" ditekan.

4. Tombol "Delete" (Menghapus Satu Data)
- Alur Tombol "Delete"
  - Cek apakah ada baris yang dipilih dalam tabel.

  - Jika ada, hapus data dari listMahasiswa berdasarkan indeks baris.

  - Perbarui tabel agar perubahan terlihat.

  - Jika tidak ada yang dipilih, tampilkan peringatan JOptionPane.

5. Tombol "Delete All" (Menghapus Semua Data)
- Alur Tombol "Delete All"
  - Cek apakah listMahasiswa kosong atau tidak.

  - Jika kosong, tampilkan pesan "Tidak ada data untuk dihapus!".

  - Jika ada data, tampilkan JOptionPane konfirmasi ("Yakin hapus semua data?").

  - Jika pengguna memilih "YES", kosongkan listMahasiswa dan perbarui tabel.

  - Tampilkan pesan sukses: "Semua data berhasil dihapus!".

6. Tombol "Cancel" (Membersihkan Form Input)
- Alur Tombol "Cancel"
  
  - Panggil metode clearForm(), yang mengosongkan semua input field.


#### RANGKUMAN ALUR KERJA
- Pengguna mengisi form (NIM, Nama, Jenis Kelamin, Angkatan).

- Menekan tombol "Add" → Data masuk ke listMahasiswa → Ditampilkan di tabel.

- Jika ingin menghapus satu data, pilih data lalu tekan tombol "Delete".

- Jika ingin menghapus semua data, tekan tombol "Delete All" → Muncul konfirmasi.

- Jika ingin mengosongkan form input, tekan tombol "Cancel".

## Dokumentasi
![Image](https://github.com/user-attachments/assets/9b8f4e8d-a653-43b3-ac3e-5187ba99be9e)

![Image](https://github.com/user-attachments/assets/9ffe6663-5a33-4f32-8211-a62076a12906)

![Image](https://github.com/user-attachments/assets/e9ef9653-6e03-4400-8326-53c004467401)

![Image](https://github.com/user-attachments/assets/f86e0943-0d84-4e3b-a7af-6833703b739b)

![Image](https://github.com/user-attachments/assets/aca7b07e-6e0b-4ea4-b814-e9ff3abee2df)

![image](https://github.com/user-attachments/assets/c1d91292-52c8-4151-b551-3fd3c6b27c0d)


