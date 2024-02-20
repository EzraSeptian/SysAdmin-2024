# Tugas week-1


1. Buat ringkasan tentang perbedaan dari Debian 12 (bookworm) dengan Debian 11 (bullseye) : versi kernel, kebutuhan sistem, penerapan systemd dan perbedaan packagenya (dalam bentuk tabel) !
2. Jelaskan fungsi dari file "/etc/groups" beserta formatnya!
3. Jelaskan perbedaan penggunaan perintah "su" dengan "su -"!
4. Jelaskan fungsi dari "sudo" !
5. Jelaskan langkah-langkah penambahan user anda sebagai user sudo ! Gunakan perintah "su -" lalu setelah masuk sebagai root, jalankan perintah "visudo". Tambahkan user anda di bawah user root pada bagian " # User privilege specification"

## Jawab
1. **Perbedaan antara Debian 12 (Bookworm) dan Debian 11 (Bullseye):**

| Fitur                           | Debian 12 (Bookworm)                               | Debian 11 (Bullseye)                             |
|---------------------------------|-----------------------------------------------------|---------------------------------------------------|
| Versi Kernel                    | Kernel 5.16                                         | Kernel 5.10                                       |
| Kebutuhan Sistem                | Mungkin lebih tinggi karena perangkat keras baru    | Stabil dan cocok untuk berbagai jenis perangkat   |
| Penerapan systemd               | Lebih dioptimalkan untuk kinerja dan manajemen      | Dukungan systemd yang stabil dan teruji          |
| Perbedaan Package               | Mungkin lebih baru dan lebih banyak versi paket     | Paket stabil dengan peningkatan perangkat terbaru |

2. **Fungsi dari file "/etc/group" beserta formatnya:**
   - File "/etc/group" adalah file konfigurasi yang mengatur informasi grup pengguna pada sistem Linux.
   - Formatnya adalah: `nama_grup:password:ID_grup:daftar_anggota`.
   - Setiap baris mewakili satu grup dan berisi informasi seperti nama grup, kata sandi terenkripsi (biasanya disimpan sebagai 'x' untuk mengindikasikan bahwa kata sandi disimpan dalam file "/etc/shadow"), ID grup, dan daftar anggota grup yang dipisahkan oleh koma.

3. **Perbedaan penggunaan perintah "su" dengan "su -":**
   - `su`: Digunakan untuk beralih pengguna tanpa mengubah variabel lingkungan (seperti $PATH, $HOME, dsb).
   - `su -`: Selain beralih pengguna, juga mengganti variabel lingkungan ke yang sesuai dengan pengguna yang baru. Ini memberikan lingkungan seperti yang dimiliki pengguna tersebut ketika pertama kali masuk.

4. **Fungsi dari "sudo":**
   - `sudo` (superuser do) adalah perintah yang memungkinkan pengguna menjalankan perintah dengan hak akses superuser atau hak akses lain yang telah ditetapkan.
   - Ini memungkinkan administrator sistem untuk memberikan akses terbatas kepada pengguna biasa untuk menjalankan perintah tertentu dengan hak akses tambahan tanpa harus memberikan akses root secara langsung.
   - Pengguna yang disebutkan dalam konfigurasi `sudoers` diizinkan untuk menjalankan perintah tertentu dengan `sudo`, memberikan lapisan keamanan tambahan dan mengurangi risiko penggunaan root secara tidak perlu.


## Langkah langkah penambahan user sudo


1. Buka terminal
2. Ketikkan su - dan masukkan password untuk root
3. Kemudian ketikkan visudo dan tambahkan your_username (4x spasi) ALL=(ALL:ALL) ALL seperti dibawah ini.

  ![gambar](asset/debian20.PNG)

4. Setelah itu tekan CTRL+O untuk overwrite dan tekan enter
5. Lalu exit dengan cara menekan CTRL+X.
6. Lalu untuk mengecek apakah user yang telah tertambah bisa menggunakan sudo, lakukan perintah sudo contoh sudo apt update, jika tidak perlu memasukkan password root maka user sudah bisa melakukan sudo
  ![gambar](asset/debian21.PNG)
