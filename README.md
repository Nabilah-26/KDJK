# Projek_KDJK_kel5_P1

# Aplikasi Web "LINKDING"

## Sekilas Tentang Linkding

**Linkding** adalah sebuah aplikasi bookmark  manager berbasis web yang gratis dan *open-source*. Aplikasi in dikembangkan untuk membantu pengguna menyimpan, mengelola, serta mengakses tautan favorit mereka dengan mudah dan efisien. Nama “Linkding” berasal dari gabungan kata *link* (tautan) dan *ding* (sebuah kata dalam bahasa jerman yang berarti “benda”), yang menggambarkan fungsinya sebagai alat untuk mengorganisasi tautan. Linkding juga mendukung impor dan ekspor bookmark dalam format HTML Netscape, serta bisa diakses melalui ekstensi peramban, bookmarklet, REST API, maupun diinstal sebagai *Progressive WebApp* (PWA). Dilengkapi dengan panel admin untuk mengelola data dan layanan mandiri pengguna, Linkding menjadi solusi ideal bagi siapa pun yang ingin menjaga koleksi tautan tetap teratur, aman, dan mudah diakses.


## Instalasi

code 1
```
int main{
  //code
}
```

code 2
```
services:
  alpha:
    env_file: ".env"
    image: joepmeneer/atomic-server:develop
    container_name: alpha
    hostname: alpha
    environment:
      - ATOMIC_DOMAIN=k5p1.online
      - ATOMIC_INITIALIZE=true
    ports:
      - "80:80"
      - "443:443"
    volumes:
      - atomic-storage:/atomic-storage
    restart: unless-stopped

volumes:
  atomic-storage:
```

## Cara Pemakaian

- Tampilan aplikasi web
1. Landing Page
   ![Halaman utama](https://github.com/bunyamin88/Projek_KDJK_kel5_P1/blob/main/SS%20Web/Screenshot%202024-10-10%20140835.png)
   Tampilan utama aplikasi web memberikan pengguna akses langsung ke fitur-fitur utama aplikasi. Pada halaman ini, pengguna dapat melihat menu navigasi, dan dari sana pengguna bisa mengakses berbagai bagian aplikasi seperti koleksi data dan lainnya.

- Fungsi-fungsi utama
2. Login
   ![Halaman user](https://github.com/bunyamin88/Projek_KDJK_kel5_P1/blob/main/SS%20Web/Screenshot%202024-10-10%20142736.png)
   Untuk dapat menggunakan fitur secara penuh, pengguna perlu melakukan login. Di halaman user settings ini, pengguna akan melakukan autentikasi, biasanya dengan username dan password yang telah ditentukan.
   
3. Collections
   ![Halaman Collection](https://github.com/bunyamin88/Projek_KDJK_kel5_P1/blob/main/SS%20Web/Screenshot%202024-10-10%20191618.png)
   xxx
   
- Isi dengan data real/dummy (jangan kosongan) dan sertakan beberapa screenshot
4. Create New Data
   ![membuat data 1](https://github.com/bunyamin88/Projek_KDJK_kel5_P1/blob/main/SS%20Web/Screenshot%202024-10-10%20192004.png)
   ![membuat data 2](https://github.com/bunyamin88/Projek_KDJK_kel5_P1/blob/main/SS%20Web/Screenshot%202024-10-10%20192102.png)
  xxx
  
5. Customize
   ![Halaman kustomisasi](https://github.com/bunyamin88/Projek_KDJK_kel5_P1/blob/main/SS%20Web/Screenshot%202024-10-10%20191645.png)
   Aplikasi ini memungkinkan pengguna untuk mengkustomisasi tampilan web sesuai dengan preferensi mereka. Pengguna dapat mengubah tema, tata letak, atau warna antarmuka aplikasi.
   
6. Shortcut
    ![Shortcut](https://github.com/bunyamin88/Projek_KDJK_kel5_P1/blob/main/SS%20Web/Screenshot%202024-10-10%20191656.png)
   xxxx

**Tips Penggunaaan**: 
Untuk memaksimalkan penggunaan aplikasi web ini, pastikan untuk login terlebih dahulu agar dapat mengakses semua fitur, serta gunakan shortcut untuk navigasi yang lebih cepat. Di bagian *Collections*, kelola data dengan cermat dan selalu simpan perubahan setelah mengedit. Jika baru mencoba fitur baru, gunakan data dummy terlebih dahulu agar data real tetap aman. Manfaatkan fitur kustomisasi tampilan, seperti *dark mode* atau pengaturan font, untuk kenyamanan penggunaan, terutama jika digunakan dalam waktu lama. Terakhir, pantau log aktivitas secara berkala untuk memantau perubahan atau aktivitas yang terjadi di aplikasi.

## Fitur/Penggunaan App
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
“Search for words or #tags” disini kita bisa mengetik kata kunci atau tag seperti “tugas” atau “#2” untuk memfilter bookmark tertentu. Fitur ini membantu pengguna menemukan link dengan cepat tanpa harus scroll panjang.

### Tags (kanan bawah)
Terdapat dua tag aktif:
2
Nala

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


## Pembahasan
Linkding adalah aplikasi web open-source untuk mengelola dan menyimpan tautan atau bookmark. Fungsinya mirip seperti layanan “Pocket” atau “Raindrop.io”, namun Linkding bisa di-host secara mandiri di server pribadi atau platform seperti Docker dan Railway. Aplikasi ini memungkinkan pengguna untuk menyimpan, menandai (tag), mencari, dan mengelola koleksi tautan dari berbagai sumber dengan cepat dan efisien. Selain itu, Linkding memiliki antarmuka sederhana dan ringan, sehingga cocok digunakan untuk pengguna pribadi maupun tim kecil yang ingin mengarsipkan referensi daring mereka.

Menurut saya, Linkding merupakan solusi yang ideal untuk pengguna yang ingin mengelola bookmark secara mandiri tanpa harus bergantung pada layanan komersial.
Aplikasi ini menawarkan keseimbangan antara kesederhanaan tampilan, kecepatan akses, dan fitur-fitur penting yang dibutuhkan pengguna sehari-hari seperti tag, pencarian cepat, serta ekstensi browser untuk menambahkan tautan langsung. Selain itu, karena bersifat open-source, aplikasi ini mudah dimodifikasi dan disesuaikan untuk kebutuhan pribadi. Namun bagi pengguna awam, proses instalasi awal bisa terasa cukup rumit karena melibatkan konfigurasi Docker, database, atau environment variable.

### Kelebihan Linkding

1. **Open-source dan gratis** – bisa digunakan tanpa biaya lisensi dan dikustomisasi sesuai kebutuhan.
2. **Ringan dan cepat** – antarmuka minimalis membuat performanya efisien bahkan di server kecil.
3. **Mendukung tag dan pencarian cepat** – memudahkan pengelompokan dan pencarian bookmark.
4. **Bisa di-host sendiri (self-hosted)** – pengguna memiliki kendali penuh terhadap data tanpa risiko privasi dari pihak ketiga.
5. **Ekstensi browser & API** – mendukung penambahan bookmark langsung dari Chrome, Firefox, atau melalui API.
6. **Mendukung multi-user** – bisa digunakan bersama dalam satu server dengan akun berbeda.
7. **Mendukung integrasi database** – kompatibel dengan SQLite untuk penggunaan sederhana dan PostgreSQL untuk skala lebih besar.
   
### Kekurangan Linkding

1. **Proses instalasi cukup teknis** – butuh pemahaman dasar tentang Docker dan konfigurasi environment.
2. **Tampilan antarmuka sangat sederhana** – meski ringan, tampilannya kurang menarik bagi sebagian pengguna.
3. **Tidak memiliki fitur backup otomatis berbasis cloud** – pengguna harus melakukan backup manual.
4. **Fitur kolaborasi terbatas** – tidak ada sistem berbagi bookmark real-time antar pengguna seperti di aplikasi berbasis cloud.
5. **Kurang integrasi sosial** – tidak seperti Pocket atau Raindrop.io yang memungkinkan berbagi ke komunitas.

### Perbandingan Linkding dengan Aplikasi Web Sejenis

#### 1. **Linkding vs Raindrop.io**

| Aspek                            | Linkding                                                  | Raindrop.io                          |
| -------------------------------- | --------------------------------------------------------- | ------------------------------------ |
| **Hosting**                      | Self-hosted, bisa dijalankan di Railway, Docker, atau VPS | Berbasis cloud                       |
| **Kustomisasi**                  | Bebas modifikasi karena open-source                       | Tidak bisa diubah (tertutup)         |
| **Sinkronisasi antar perangkat** | Manual (via server sendiri)                               | Otomatis dan real-time               |
| **Tampilan UI**                  | Minimalis, fungsional                                     | Sangat modern dan estetis            |
| **Dukungan ekstensi browser**    | Ya                                                        | Ya                                   |
| **Fitur kolaborasi**             | Terbatas                                                  | Ada fitur tim dan folder kolaboratif |

Kesimpulan: Pocket lebih ramah bagi pengguna umum, tapi Linkding unggul dalam hal privasi dan kendali data pribadi.

#### 2. **Linkding vs Pocket**

| Aspek                    | Linkding                            | Pocket                                               |
| ------------------------ | ----------------------------------- | ---------------------------------------------------- |
| **Kepemilikan Data**     | Self-hosted (data milik pengguna)   | Data disimpan di server Pocket                       |
| **Biaya**                | Gratis (open-source)                | Gratis dengan fitur terbatas, versi premium berbayar |
| **Privasi**              | Sangat tinggi karena server pribadi | Bergantung pada kebijakan Pocket                     |
| **Antarmuka**            | Sederhana dan ringan                | Lebih modern dan interaktif                          |
| **Fitur tambahan**       | Tag, pencarian cepat, API           | Artikel rekomendasi, highlight teks, sinkronisasi    |
| **Kemudahan penggunaan** | Butuh setup manual (Docker)         | Siap pakai (langsung registrasi)                     |

Kesimpulan: Raindrop.io lebih unggul untuk kolaborasi dan tampilan modern, tetapi Linkding lebih cocok bagi pengguna yang mengutamakan privasi, kontrol penuh, dan kecepatan.

## Kesimpulan

Atomic Data menawarkan fleksibilitas tinggi dalam pengelolaan data terstruktur dengan skema yang fleksibel, validasi tipe yang ketat, serta kemampuan audit dan versioning yang baik. Namun, untuk kasus penggunaan tertentu seperti skala besar, data internal, atau data multimedia, aplikasi lain seperti RDF, JSON-LD, dan GraphQL mungkin lebih tepat digunakan. Atomic Data unggul dalam kasus di mana interoperabilitas, auditabilitas, dan konektivitas data terdesentralisasi sangat dibutuhkan.


## Referensi

(https://docs.atomicdata.dev/)
