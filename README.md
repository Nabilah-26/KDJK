# Project KDJK Kel9 P1

# Aplikasi Web "LINKDING"

## Sekilas Tentang Linkding

**Linkding** adalah sebuah aplikasi bookmark  manager berbasis web yang gratis dan *open-source*. Aplikasi ini dikembangkan untuk membantu pengguna menyimpan, mengelola, serta mengakses tautan favorit mereka dengan mudah dan efisien. Nama “Linkding” berasal dari gabungan kata *link* (tautan) dan *ding* (sebuah kata dalam bahasa jerman yang berarti “benda”), yang menggambarkan fungsinya sebagai alat untuk mengorganisasi tautan. Linkding juga mendukung impor dan ekspor bookmark dalam format HTML Netscape, serta bisa diakses melalui ekstensi peramban, bookmarklet, REST API, maupun diinstal sebagai *Progressive WebApp* (PWA). Linkding menjadi solusi ideal bagi siapa pun yang ingin menjaga koleksi tautan tetap teratur, aman, dan mudah diakses.


## Instalasi 
# 🚀 Panduan Deploy Linkding di Railway

<p align="center">
  <img src="https://github.com/user-attachments/assets/b3558f1a-b66b-4077-85f0-88dded4af6a6" alt="Langkah 1" width="45%" />
  <img src="https://github.com/user-attachments/assets/1c555b76-f3c7-4637-857b-b35d89ee3104" alt="Langkah 2" width="45%" />
</p>


1. Buka situs [**railway.com**](https://railway.com), kemudian tekan **Sign In** di kanan atas.  
2. Lakukan **Sign In** menggunakan akun **GitHub** atau **Email**.  

<p align="center">
  <img src="https://github.com/user-attachments/assets/0432ff09-9b0b-4009-b0e4-1c1e5eb277d9" alt="Langkah 3" width="45%" />
  <img src="https://github.com/user-attachments/assets/86563b2c-eb4c-44db-b4ba-3c9d27c519fc" alt="Langkah 4" width="45%" />
</p>

3. Setelah berhasil masuk, buka **Dashboard** di kanan atas.  
4. Tekan tombol **Create New Project**.  

<p align="center">
  <img src="https://github.com/user-attachments/assets/2f4d8e08-64e2-41e1-84c7-7bccb2b664b6" alt="Langkah 5" width="45%" />
  <img src="https://github.com/user-attachments/assets/10120648-94a5-46b5-b3f6-1b0d72d0a098" alt="Langkah 6" width="45%" />
</p>

5. Pilih opsi **Docker Image**.  
6. Masukkan `sissbruecker/linkding:1.44.1-plus-alpine` sebagai sumber image Linkding.  

<p align="center">
  <img src="https://github.com/user-attachments/assets/70510fe0-6bde-48a8-a627-568642952b0b" alt="Langkah 7" width="45%" />
  <img src="https://github.com/user-attachments/assets/faa826f2-193e-494c-b995-4286e62e50eb" alt="Langkah 8" width="45%" />
</p>

7. Tunggu hingga Railway memuat Docker image Linkding.  
8. Setelah image berhasil dimuat, buka tab **Variables**.  

<p align="center">
  <img src="https://github.com/user-attachments/assets/756851fd-bd69-4fc5-b614-7a9ec44fb369" alt="Langkah 9" width="45%" />
  <img src="https://github.com/user-attachments/assets/6948a12d-ffc8-4ee9-8236-04e6e8ee70e0" alt="Langkah 10" width="45%" />
</p>

9. Tekan tombol **Raw Editor**.
10. Masukkan environment variable berikut:  

    ```env
    PORT="9090"
    LD_BIND_ADDRESS="0.0.0.0"
    LD_PORT="$PORT"
    LD_SUPERUSER_NAME="kelompok9"
    LD_SUPERUSER_PASSWORD="987654321"
    ```
<p align="center">
  <img src="https://github.com/user-attachments/assets/28e2fc13-254d-4e80-8e01-620c78751afa" alt="Langkah 11" width="45%" />
  <img src="https://github.com/user-attachments/assets/1cde559f-a0b0-47bb-b7d2-5133f238a1b5" alt="Langkah 12" width="45%" />
</p>

11. Tekan tombol **Update Variables** (berwarna biru).  
12. Setelah di-update, akan muncul notifikasi di kiri atas.
    
<p align="center">
  <img src="https://github.com/user-attachments/assets/5ee5b21d-5087-4db3-bb61-e06a2b91ea2a" alt="Langkah 13" width="45%" />
  <img src="https://github.com/user-attachments/assets/ecbbdcba-4e77-4272-80bd-06022ccf209b" alt="Langkah 14" width="45%" />
</p>

13. Tekan tombol **Deploy** pada notifikasi tersebut untuk menyimpan perubahan.  
14. Setelah proses deploy selesai, buka tab **Settings**.  

<p align="center">
  <img src="https://github.com/user-attachments/assets/fabb5e67-94df-44ac-8294-52c298a66f31" alt="Langkah 15" width="45%" />
  <img src="https://github.com/user-attachments/assets/70c94e7e-60d0-4214-a1e8-2ca01864b29b" alt="Langkah 16" width="45%" />
</p>

15. Pada bagian **Networking**, tekan tombol **Generate Domain** untuk membuat link situs.  
16.  **Link Hosting Linkding berhasil dideploy!**

## Fitur/Penggunaan App
<img width="1475" height="551" alt="image" src="https://github.com/user-attachments/assets/e5c2328f-ca04-4030-a28e-fec01795ce01" />

### Login Page
Pada halaman ini terdapat dua input utama dan satu tombol aksi:
- Username – digunakan untuk memasukkan nama pengguna (contoh: rifat).
- Password – kolom untuk memasukkan kata sandi.
- Tombol Login – mengeksekusi proses autentikasi agar pengguna bisa masuk ke sistem.

<img width="1519" height="740" alt="image" src="https://github.com/user-attachments/assets/5599a19f-83f2-4f64-8257-20a58e409e7d" />

### Bookmarks 
“tugassss” dan “nala” adalah dua bookmark yang berhasil ditambahkan oleh pengguna. Masing-masing bookmark memiliki tag berbeda (#2 dan #nala) untuk mengelompokkan topik.
Setiap bookmark bisa:
- View: membuka link di tab baru.
- Edit: mengubah judul, tag, atau deskripsi.
- Archive: menandai link agar tidak tampil di daftar utama.
- Remove: menghapus link dari sistem.

Ini menunjukkan bahwa fungsi CRUD (Create, Read, Update, Delete) dalam aplikasi Linkding berjalan normal.

### Kolom pencarian (search)
“Search for words or #tags” disini pengguna bisa mengetik kata kunci atau tag seperti “tugas” atau “#2” untuk memfilter bookmark tertentu. Fitur ini membantu pengguna menemukan link dengan cepat tanpa harus scroll panjang.

### Tags (kanan bawah)
Terdapat dua tag aktif:
- 2
- Nala

Tag ini muncul otomatis dari setiap bookmark yang dibuat. Klik salah satu tag (misalnya “2”), maka aplikasi hanya menampilkan bookmark dengan tag tersebut. Fungsi tag ini mirip seperti “kategori” di aplikasi pencatat atau bookmark online lainnya seperti Pocket atau Raindrop.

### Bundles (kanan atas)
Di sini muncul satu bundle bernama “nala”.
Bundle digunakan untuk mengelompokkan beberapa tag menjadi satu grup besar. Contohnya, bundle “Kuliah” bisa berisi tag #tugas, #referensi, dan #deadline. Ini memudahkan pengguna untuk mengelola banyak tag sekaligus.

### Navigasi dan antarmuka
Di bawah daftar bookmark ada navigasi: “Previous | 1 | Next”
Menandakan bahwa aplikasi sudah siap menampilkan bookmark dalam jumlah banyak dengan sistem pagination (halaman 1, 2, dst). Tombol di bagian atas:
- Add Bookmark: untuk menambah data baru.
- Settings: mengatur preferensi aplikasi (seperti API key, tampilan, dan backup data).
- Logout: keluar dari akun pengguna.

<img width="1456" height="844" alt="image" src="https://github.com/user-attachments/assets/9e3c3018-105b-4077-9c89-badd311e7529" />
<img width="1038" height="235" alt="image" src="https://github.com/user-attachments/assets/03f9e630-0f42-4348-a5b1-fb592a511545" />

### Add bookmark

Halaman ini digunakan untuk menyimpan link atau tautan penting agar mudah diakses kembali di kemudian hari.
Fungsinya mirip seperti “Save” atau “Bookmark” di browser, tetapi Linkding menyimpannya dalam satu sistem terorganisir, bisa diberi tag, deskripsi, dan status baca (read/unread).

1. URL
Kolom ini untuk menuliskan alamat situs web yang ingin disimpan. Setelah disimpan, Linkding akan menampilkan tautan tersebut di daftar bookmark.

2. Tags
Berfungsi memberi kategori atau label pada setiap bookmark. Tag membantu pengguna mengelompokkan dan mencari link dengan cepat. Ditulis tanpa tanda pagar (#), lalu cukup pisahkan dengan spasi.

Contoh: kuliah referensi kdjk

Maka Linkding akan otomatis membuat tag kuliah, referensi, dan kdjk.

4. Title
Judul dari link yang disimpan. Bisa otomatis diambil dari situs, atau diketik manual. Judul memudahkan identifikasi isi link tanpa harus membukanya.

5. Description
Tempat untuk menuliskan penjelasan singkat tentang isi link atau alasan menyimpannya.

6. Notes (opsional)
Dapat digunakan untuk menambahkan catatan pribadi seperti ringkasan atau ide penting dari link tersebut.

7. Mark as Unread
Jika dicentang, link akan ditandai sebagai belum dibaca (unread). Linkding menyediakan filter agar pengguna bisa menampilkan hanya link yang belum dibaca.

8. Tombol Save & Cancel
- Save → Menyimpan link ke dalam sistem Linkding.
- Cancel → Membatalkan proses penyimpanan dan kembali ke halaman sebelumnya.

<img width="273" height="268" alt="image" src="https://github.com/user-attachments/assets/80e58afa-9d67-432f-96b3-19914874e711" />

### Menu bookmark
berfungsi untuk mengelola dan memfilter tautan (link) yang sudah disimpan oleh pengguna.

1. Active
Menampilkan semua bookmark yang masih aktif atau belum diarsipkan. Ini adalah tampilan utama yang biasa digunakan untuk melihat semua link yang masih relevan.

Contoh penggunaan:
pengguna baru saja menyimpan artikel penting untuk tugas kuliah, dan ingin melihatnya lagi di daftar utama.

2. Archived
Berisi bookmark yang sudah disimpan tetapi tidak lagi dibutuhkan secara aktif. Cocok untuk menjaga tampilan utama tetap rapi tanpa menghapus link lama. Bookmark yang diarsipkan masih bisa dikembalikan ke status aktif jika dibutuhkan.

Contoh penggunaan:
Artikel yang sudah selesai dibaca atau digunakan dalam proyek, tetapi tetap ingin disimpan sebagai referensi.

3. Unread
Menampilkan bookmark yang sudah disimpan namun belum dibaca atau dibuka oleh pengguna. Fitur ini memudahkan pengguna untuk menyortir link yang perlu ditinjau nanti.

Contoh penggunaan:
Pengguna menandai beberapa artikel riset dengan “Mark as unread” supaya mudah ditemukan untuk dibaca nanti.

4. Untagged
Menampilkan semua bookmark yang belum memiliki tag (belum dikategorikan). Berguna untuk melakukan pengelolaan ulang agar semua link punya kategori/tag yang sesuai.

Contoh penggunaan:
Setelah menyimpan banyak link cepat-cepat, pengguna bisa buka menu ini untuk menambahkan tag pada yang belum dikategorikan.

## Pembahasan
Linkding adalah sebuah aplikasi web yang bersifat open-source, dirancang untuk mengelola dan menyimpan tautan atau bookmark. Fungsinya serupa dengan layanan seperti "Pocket" atau "Raindrop. io", tetapi Linkding memungkinkan pengguna untuk dipasang di server mereka sendiri atau di lingkungan seperti Docker dan Railway. Aplikasi ini memberikan kemampuan kepada penggunanya untuk dengan cepat dan efisien menyimpan, memberi tag, mencari, dan mengatur koleksi tautan dari berbagai sumber. Selanjutnya, Linkding memiliki antarmuka yang sederhana dan ringan, menjadikannya pilihan tepat untuk individu maupun tim kecil yang ingin mengarsipkan referensi secara online.

Saya percaya bahwa Linkding adalah solusi yang cocok bagi pengguna yang ingin melakukan pengelolaan bookmark secara mandiri tanpa tergantung pada layanan berbayar. Aplikasi ini menciptakan keseimbangan antara kesederhanaan tampilan, kecepatan, dan fitur-fitur esensial yang diperlukan pengguna sehari-hari, seperti penandaan, pencarian cepat, serta ekstensi browser untuk menambah tautan secara langsung. Selain itu, dengan sifat open-source nya, aplikasi ini dapat dengan mudah disesuaikan dan dimodifikasi sesuai kebutuhan pengguna. Namun, pengguna yang kurang berpengalaman mungkin menemukan bahwa instalasi awal bisa menjadi agak rumit karena perlu konfigurasi Docker, database, atau variabel lingkungan.

### Kelebihan Linkding

1. **Open-source dan gratis** – Linkding dapat dimanfaatkan tanpa pembayaran lisensi serta disesuaikan berdasarkan kebutuhan pengguna.
2. **Ringan dan responsif** – Tampilan Linkding yang sederhana membuat kinerjanya optimal bahkan pada server yang kecil.
3. **Mendukung tagging dan pencarian cepat** – Linkding mempermudah dalam mengelompokkan dan mencari bookmark.
4. **Dapat di-hosting sendiri (self-hosted)** – Linkding dapat dihosting oleh masing-masing user sehingga memiliki kontrol penuh atas data tanpa menghadapi risiko privasi dari pihak ketiga.
5. **Ekstensi browser & API** – Linkding mendukung penambahan bookmark secara langsung dari Chrome, Firefox, atau melalui API.
6. **Mendukung multi-user** – Linkding dapat diakses secara bersamaan di satu server dengan akun yang berbeda.
   
### Kekurangan Linkding

1. **Proses instalasi cukup rumit** – Proses penginstalan Linkding memerlukan pengetahuan dasar mengenai Docker dan Konfigurasi environment.
2. **Tampilan antarmuka sangat sederhana** –  Walaupun ringan, Desain Linkding kurang menarik bagi sebagian user.
3. **Tidak dilengkapi dengan fitur pencadangan otomatis berbasis cloud** – Pengguna Linkding diwajibkan untuk melakukan pencadangan secara manual.
4. **Fitur kolaborasi terbatas** – Dalam Linkding tidak terdapat sistem berbagi bookmark secara real-time antara pengguna seperti yang ada dalam aplikasi berbasis cloud.
5. **Kurang adanya integrasi sosial** – Linkding tidak seperti Pocket atau Raindrop. io yang menyediakan opsi untuk berbagi dengan komunitas.

### Perbandingan Linkding dengan Aplikasi Web Sejenis

#### 1. **Linkding vs Shaarli**

| Aspek                         | Linkding                                                         | Shaarli                                                                 
| ----------------------------- | ---------------------------------------------------------------- | ----------------------------------------------------------------------- 
| **Hosting**                   | Self-hosted berbasis Docker, bisa dijalankan di Railway atau VPS | Self-hosted, sangat ringan dan bisa dijalankan langsung di server kecil 
| **Bahasa Pemrograman**        | Python (Django)                                                  | PHP (tanpa framework besar)                                             
| **Kustomisasi**               | Dapat dimodifikasi, memiliki API dan dukungan ekstensi           | Sangat mudah diubah karena struktur kode sederhana                      
| **Kinerja**                   | Stabil, tapi butuh resource sedikit lebih tinggi                 | Sangat cepat dan ringan, cocok untuk server kecil                       
| **Antarmuka (UI)**            | Minimalis dan modern                                             | Sangat sederhana, fokus pada fungsi dasar                               
| **Fitur utama**               | Tagging, pencarian cepat, impor/ekspor bookmark, API             | Simpan dan kelola tautan pribadi dengan cepat                           
| **Fitur kolaborasi**          | Terbatas (satu pengguna utama)                                   | Tidak mendukung multi-user secara default                               
| **Dukungan ekstensi browser** | Ya, tersedia untuk Chrome & Firefox                              | Ya, tapi sangat dasar (manual save via bookmarklet)                     

Kesimpulan : Shaarli unggul dalam kecepatan dan kesederhanaan, sangat cocok untuk pengguna yang ingin bookmark pribadi tanpa ribet. Namun, Linkding menawarkan pengalaman yang lebih modern dengan fitur tambahan seperti tagging, API, dan antarmuka yang lebih rapi.

#### 2. **Linkding vs Linkwarden**

| Aspek                      | Linkding                                | Linkwarden                                                 |
| -------------------------- | --------------------------------------- | ---------------------------------------------------------- |
| **Hosting**                | Self-hosted, bisa dijalankan via Docker | Self-hosted berbasis Node.js + MongoDB                     |
| **Bahasa Pemrograman**     | Python (Django)                         | TypeScript / Next.js                                       |
| **Kustomisasi**            | Cukup fleksibel, open-source            | Sangat fleksibel, open-source dan modular                  |
| **Antarmuka (UI)**         | Sederhana dan minimalis                 | Lebih modern dan interaktif dengan tampilan bergaya Notion |
| **Fitur kolaborasi**       | Terbatas (single user)                  | Ada fitur multi-user dan kolaboratif                       |
| **Fitur tambahan**         | Tagging, impor/ekspor, API sederhana    | Simpan snapshot halaman (HTML, PDF, screenshot), anotasi   |
| **Kinerja**                | Ringan, cepat pada deployment kecil     | Lebih berat karena fitur arsip dan visualisasi konten      |
| **Privasi & kontrol data** | Penuh (karena self-hosted)              | Penuh (juga self-hosted)                                   |
| **Kemudahan setup**        | Mudah dengan Docker                     | Setup lebih kompleks (butuh konfigurasi database dan env)  |

Kesimpulan:
Linkwarden unggul dalam fitur kolaboratif dan kemampuan arsip halaman (menyimpan konten, bukan hanya link). Namun, Linkding lebih ringan dan mudah dijalankan, cocok bagi pengguna yang menginginkan bookmark manager pribadi tanpa kompleksitas tambahan.

## Kesimpulan
Proyek ini berhasil mendemonstrasikan bagaimana aplikasi Linkding dapat di-deploy dan dijalankan melalui platform Railway sebagai solusi manajemen bookmark berbasis web yang ringan, cepat, dan mudah digunakan. Linkding menghadirkan keseimbangan antara kesederhanaan dan fungsionalitas, dengan kemampuan untuk menyimpan, menandai (tagging), dan mencari tautan secara efisien. Selama proses implementasi, terbukti bahwa Linkding dapat berjalan dengan baik meskipun tanpa konfigurasi database kompleks, menjadikannya cocok untuk kebutuhan personal maupun kelompok kecil. Aplikasi ini juga menunjukkan keunggulan dalam hal kontrol data pribadi, karena pengguna dapat melakukan self-hosting dan sepenuhnya memiliki kendali atas datanya sendiri.

Dari sisi perbandingan, hasil analisis menunjukkan bahwa:
1. Dibandingkan dengan Shaarli, Linkding lebih modern dan kaya fitur meskipun sedikit lebih berat.
2. Dibandingkan dengan Linkwarden, Linkding lebih ringan dan mudah di-deploy, walaupun tidak sekompleks Linkwarden yang memiliki fitur kolaboratif dan arsip halaman.

Secara keseluruhan, Linkding merupakan pilihan ideal bagi pengguna yang ingin memiliki sistem manajemen bookmark mandiri, aman, dan efisien tanpa ketergantungan pada layanan pihak ketiga. Walaupun memiliki keterbatasan pada sisi tampilan dan kolaborasi, Linkding menawarkan fondasi kuat untuk pengelolaan tautan berbasis privasi dan fleksibilitas penuh dalam pengembangan.

## Referensi
https://hub.docker.com/r/sissbruecker/linkding
https://linkwarden.app/
https://github.com/shaarli/Shaarli
https://linkding.link/

