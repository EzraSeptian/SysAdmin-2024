    NRP   : 3122600016
    Nama  : Ezra Septian Handyanto
    Kelas : 2 D4 IT A
    Dosen : Dr. Ferry Astika Saputra, ST, M.Sc

# Bagaimana Internet bisa berkembang dengan pesat di seluruh dunia ?

Kesuksesan Internet yang belum pernah terjadi sebelumnya terus berkembang karena model Internet yang terbuka, transparan, dan kolaboratif  mengandalkan proses dan produk yang bersifat lokal, bottom-up, dan dapat diakses oleh pengguna di seluruh dunia.

- Tiga Kunci sukses Internet:
  - kepemilikan global Bersama
  - pengembangan standar terbuka
  - proses pengembangan teknologi dan kebijakan yang dapat diakses secara bebas.

## Internet dapat dipandang dari 2 sisi

- Teknis

  - Routing system (system routing)

    - Routing system merupakan salah satu komponen kunci dalam infrastruktur internet yang memungkinkan pengiriman data antara berbagai perangkat dan jaringan. Ini bekerja dengan mengarahkan paket data melalui jaringan yang paling efisien dan dapat diandalkan dari sumber ke tujuan. Teknik routing system pada internet melibatkan serangkaian algoritma dan protokol yang kompleks untuk mengoptimalkan pengiriman data.

    Berikut adalah beberapa teknik utama dalam routing system pada internet:

    1. **Routing Protocols**: Routing protocols adalah perangkat lunak atau algoritma yang digunakan router untuk bertukar informasi tentang jaringan yang terhubung. Ini memungkinkan router untuk memahami topologi jaringan dan memutuskan rute terbaik untuk mengirim paket data. Beberapa protokol routing yang umum digunakan di Internet termasuk:

       - **Border Gateway Protocol (BGP)**: Digunakan untuk routing antar-doman di Internet. BGP adalah protokol yang sangat kompleks dan hierarkis yang digunakan oleh penyedia layanan internet (ISP) dan jaringan besar lainnya untuk membuat keputusan tentang rute terbaik untuk mencapai tujuan tertentu di internet.

       - **Open Shortest Path First (OSPF)**: Protokol routing interior yang digunakan dalam jaringan IP berskala besar seperti perusahaan dan penyedia layanan internet. OSPF menggunakan algoritma Dijkstra untuk menemukan rute terpendek antara dua node di jaringan.

       - **Routing Information Protocol (RIP)**: Protokol routing interior yang sederhana dan sering digunakan dalam jaringan kecil. RIP menggunakan algoritma Bellman-Ford untuk menentukan rute terbaik.

    2. **Algoritma Routing**: Algoritma routing adalah pendekatan matematis yang digunakan oleh router untuk memutuskan rute terbaik untuk mengirim paket data. Beberapa algoritma routing yang umum digunakan termasuk:

       - **Distance Vector**: Algoritma routing yang digunakan oleh protokol seperti RIP. Router bertukar informasi tentang jaringan yang terhubung dan memutuskan rute berdasarkan jumlah "hops" atau node antara sumber dan tujuan.

       - **Link State**: Algoritma routing yang digunakan oleh protokol seperti OSPF. Setiap router membangun peta lengkap dari topologi jaringan dan menggunakan informasi ini untuk menghitung rute terpendek ke setiap tujuan.

    3. **Pengukuran dan Pemantauan Jaringan**: Penting untuk terus memantau kinerja jaringan dan mengukur berbagai parameter seperti lalu lintas, latensi, dan keandalan koneksi. Ini membantu router dalam membuat keputusan yang lebih baik tentang rute terbaik untuk mengirim paket data.

    4. **Penggunaan Metrik**: Router menggunakan metrik untuk mengevaluasi kualitas dan efisiensi rute yang tersedia. Metrik ini dapat mencakup berbagai faktor seperti bandwidth, kecepatan, biaya, dan keandalan.

    5. **Penanganan Kondisi Darurat**: Routing system harus mampu menangani kondisi darurat seperti kegagalan jaringan atau router. Ini dapat dilakukan dengan menggunakan teknik seperti rerouting otomatis atau peningkatan jalur cadangan.

    6. **Penggunaan Jalur Ganda**: Beberapa router dapat menggunakan jalur ganda untuk meningkatkan ketersediaan dan throughput jaringan. Teknik seperti Equal-Cost Multipath (ECMP) memungkinkan router untuk membagi lalu lintas antara beberapa jalur dengan biaya yang sama.

    Routing system pada internet terus berkembang dan kompleksitasnya meningkat seiring dengan pertumbuhan jaringan dan kebutuhan pengguna. Ini memerlukan penelitian dan pengembangan terus-menerus untuk menjaga kinerja dan keandalan infrastruktur internet.

  - Naming system (sistem penamaan)

    - Naming system pada internet merujuk pada cara pengenal dan penamaan alamat dan sumber daya yang ada di jaringan. Salah satu aspek paling penting dari sistem ini adalah Domain Name System (DNS), yang merupakan bagian integral dari bagaimana internet berfungsi. Berikut adalah penjelasan rinci tentang nama sistem pada internet:

    1. **Domain Name System (DNS)**:

    - DNS adalah sistem hierarkis yang mengaitkan nama domain yang mudah diingat dengan alamat IP numerik yang digunakan oleh komputer dan perangkat di internet.
    - Ini memungkinkan pengguna untuk mengakses situs web dan layanan online dengan mengetikkan nama domain yang mudah diingat, seperti "google.com", alih-alih harus mengingat alamat IP numerik yang panjang.
    - DNS terdiri dari beberapa komponen, termasuk server DNS, zona DNS, dan rekaman DNS seperti A (alamat IPv4), AAAA (alamat IPv6), MX (penerima email), CNAME (alias), dan lain-lain.
    - Saat pengguna memasukkan nama domain ke dalam browser, perangkat klien mengirim permintaan DNS ke server DNS lokalnya untuk mencari alamat IP terkait. Jika tidak ditemukan di server lokal, permintaan akan dikirim ke server DNS yang lebih tinggi dalam hierarki, dan seterusnya, hingga alamat IP ditemukan dan dikirim kembali ke klien.

    2. **Uniform Resource Locator (URL)**:

    - URL adalah cara standar untuk menunjukkan lokasi sumber daya di internet. Ini umumnya digunakan untuk mengakses halaman web, tetapi juga dapat mengacu pada berbagai jenis sumber daya online lainnya, seperti gambar, video, atau dokumen.
    - URL terdiri dari beberapa bagian, termasuk skema (misalnya HTTP atau HTTPS), nama domain, jalur, dan parameter opsional. Contohnya adalah "https://www.example.com/page1".

    3. **Uniform Resource Identifier (URI)**:

    - URI adalah konsep yang lebih umum daripada URL. Ini adalah string karakter yang digunakan untuk mengidentifikasi sumber daya secara unik, baik di internet maupun di luar internet. URL adalah jenis URI yang menentukan lokasi sumber daya secara spesifik.

    4. **Internet Protocol (IP) Addresses**:

    - IP address adalah alamat numerik yang diberikan kepada setiap perangkat yang terhubung ke jaringan internet. Ada dua versi utama dari alamat IP yang digunakan saat ini: IPv4 dan IPv6.
    - IPv4 menggunakan format yang lebih tua dan terdiri dari empat bagian angka desimal dipisahkan oleh titik, misalnya "192.0.2.1".
    - IPv6 adalah versi yang lebih baru dan menggunakan format yang lebih panjang dan kompleks yang terdiri dari delapan grup digit heksadesimal, misalnya "2001:0db8:85a3:0000:0000:8a2e:0370:7334".

    5. **Internationalized Domain Names (IDN)**:

    - IDN adalah nama domain yang mengandung karakter non-ASCII, seperti aksara internasional atau karakter skrip non-Latin. Ini memungkinkan pengguna untuk menggunakan nama domain dalam bahasa mereka sendiri, meningkatkan aksesibilitas dan inklusivitas internet.
    - Contoh IDN adalah nama domain dalam aksara Rusia atau Cina.

    6. **Top-Level Domain (TLD)**:

    - TLD adalah bagian paling kanan dari sebuah nama domain, seperti ".com", ".org", atau ".net". Ini menunjukkan jenis organisasi atau tujuan dari nama domain tersebut.

    Naming system pada internet adalah fondasi dari bagaimana pengguna mengakses dan berinteraksi dengan sumber daya online. Ini memungkinkan pengguna untuk dengan mudah mengidentifikasi dan mengakses situs web, layanan, dan sumber daya lainnya tanpa harus mengingat alamat IP numerik yang rumit.

- Arsitektur
  - Standards (standarisasi)
  - Service Providers (penyedia layanan) • Internet Registries (Internet register) • Clearing Houses (Rumah kliring)
