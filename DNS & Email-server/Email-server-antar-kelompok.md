    NRP   : 3122600016
    Nama  : Ezra Septian Handyanto
    Kelas : 2 D4 IT A
    Dosen : Dr. Ferry Astika Saputra, ST, M.Sc

# Langkah - langkah

1. Pertama pastikan resolv.conf terdapat search kelompok3.local, setelah itu masukkan perintah telnet mail.kelompok3.local 25 untuk mengirim pesan
   ke kelompok lain
2. Setelah itu ketikkan 
   MAIL FROM: <pengirim@kelompok3.local>

   RCPT TO:<penerima@kelompok2.local>

   DATA
   halo saya dari kelompok3.local

   . (untuk mengakhiri session ngirim email: . kemudian enter)

   QUIT (untuk mengakhiri session email)

3. Kemudian cek mail di device penerima dengan 2 cara melalui evolution atau menggunakan terminal:
   1. Buka melalui evolution, pastikan akun yang terlogin sesuai dengan yang menerima email kemudian cek pada inbox jika berhasil menerima mail
      maka akan muncul seperti ini:
      
      Menerima mail dari kelompok3.local:

      ![gambar](asset/sent-telnet.jpg)

      Menerima mail dari kelompok2.local:

      ![gambar](asset/received-evolution.jpg)

   2. Kemudian jika kita cek pada terminal menggunakan perintah
      telnet kelompok3.local 110
      
      user username (sesuaikan dengan username di debian)
      
      pass password (sesuaikan dengan password di debian)
      
      list (memunculkan list email yang ada di debian)
      
      retr nomerlist (ganti nomerlist sesuai dengan mail yang ingin diperiksa)
      
      quit (jika dirasa sudah cukup)
      
      ![gambar](asset/received-telnet.jpg)

 # Roundcube

1. Install with `sudo apt install roundcube`

   ![Screenshot 2024-04-30 085423](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/a444894c-5992-4f2d-a98b-627b90814d9b)

   ![Screenshot 2024-04-30 085431](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/fc135aa3-9318-468a-928c-59dff4a70006)

2. Membuat Database User di MariaDB

   ![Screenshot 2024-04-30 090056](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/1aa540cb-86d7-4b1a-83c2-97ec4a2e6ae8)

3. Konfigurasi

   ![Screenshot 2024-04-30 090253](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/9d1c061b-e0c1-476f-9301-ca755070bb5b)

   ![Screenshot 2024-04-30 090804](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/dcd78ddf-8a57-41bc-8feb-0027690f6f2f)

   ![Screenshot 2024-04-30 090720](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/39680c7b-93bc-46c4-b3ec-6e6916ca1924)

   ![Screenshot 2024-04-30 090928](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/63a7c093-0fc5-4019-b0ad-e0ff3ea60223)

   ![Screenshot 2024-04-30 090951](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/131f68ea-cc9a-48ae-9afb-ebc84e48c3a6)

   ![Screenshot 2024-04-30 091004](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/19bcfae1-000f-4f32-92cc-65004a17c34b)

   ![Screenshot 2024-04-30 091018](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/6d2eef88-a1bc-4b9b-921e-d355454f5c81)

   ![Screenshot 2024-04-30 091033](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/a35b072e-f253-41d4-b79e-4ee0e8ae677b)

   ![Screenshot 2024-04-30 091109](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/91edfa3e-eec3-4ae1-89d8-7639540dca3d)

   ![Screenshot 2024-04-30 091126](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/1ae50a58-151b-4b04-919a-4d8accd54ff1)

4. Final Check

   ![Screenshot 2024-04-30 091244](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/e555dc3f-c4a6-46a6-bbf6-382c61b7a2cb)

   ![Screenshot 2024-04-30 091302](https://github.com/Mahargip/SysAdmin_2024/assets/114201452/25a24201-aeda-4574-9363-301999ef1fa4)
   
