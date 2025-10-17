# Projek_KDJK_kel5_P1

# Aplikasi Web "LINKDING"

## Sekilas Tentang

xxys


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


## Pembahasan
### Kelebihan Atomic Data

1. **Skema Fleksibel**: Atomic Data sangat cocok untuk data yang bervariasi, seperti wiki terstruktur atau data semantik, karena memungkinkan setiap objek memiliki atribut yang berbeda. Setiap sumber daya dapat memiliki properti yang berbeda sesuai kebutuhan.

### Kekurangan Atomic Data

1. **Penggunaan Internal Saja**: Jika data hanya digunakan secara internal dan tidak perlu dibagikan kepada pihak luar, menggunakan Atomic Data justru dapat mempersulit proses karena sifatnya yang lebih kompleks dibandingkan format lain seperti JSON.

### Perbandingan Atomic Data dengan Aplikasi Web Sejenis

#### 1. **Atomic Data vs JSON-LD**

- **Kelebihan Atomic Data:**
  - **Skema Fleksibel**: Atomic Data memungkinkan penambahan properti apapun pada sumber daya, yang membuatnya lebih dinamis dalam menangani berbagai jenis data.
  - **Validasi Tipe Data**: Atomic Data menggunakan tipe data yang terstruktur dengan baik, sehingga setiap nilai harus divalidasi berdasarkan tipe datanya, memberikan keamanan yang lebih tinggi.
  - **Auditabilitas dan Versi**: Atomic Data mendukung Atomic Commits, yang memungkinkan penyimpanan setiap perubahan sebagai transaksi, memberikan kemampuan audit dan riwayat perubahan yang terperinci.

- **Kelebihan JSON-LD:**
  - **Kompatibilitas**: JSON-LD lebih populer dan didukung oleh berbagai platform seperti Google dan aplikasi web yang membutuhkan data terstruktur untuk SEO.
  - **Kemudahan Penggunaan**: JSON-LD lebih mudah digunakan dan diterapkan karena strukturnya yang lebih sederhana dan langsung dapat diintegrasikan dengan JSON biasa.
  - **Kinerja**: JSON-LD lebih ringan karena tidak memerlukan validasi tipe yang ketat seperti Atomic Data, sehingga lebih cepat dalam memproses data yang sederhana.

#### 2. **Atomic Data vs RDF (Resource Description Framework)**

- **Kelebihan Atomic Data:**
  - **Kemudahan Implementasi**: Atomic Data lebih mudah diimplementasikan dibandingkan RDF, karena strukturnya lebih modular dan sederhana.
  - **Penggunaan URL untuk Dokumentasi**: Atomic Data menggunakan URL untuk mendokumentasikan properti, menjadikan data lebih mudah dimengerti tanpa memerlukan dokumentasi eksternal tambahan.
  - **Fleksibilitas**: Atomic Data memberikan fleksibilitas yang lebih tinggi dalam menentukan skema dan properti yang dapat digunakan oleh berbagai sumber data.

- **Kelebihan RDF:**
  - **Standar Terbuka**: RDF telah menjadi standar untuk data terstruktur yang terhubung di web, dengan dukungan dari berbagai organisasi dan platform.
  - **Skalabilitas untuk Dataset Besar**: RDF lebih cocok untuk skala besar, seperti Big Data dan dataset terdistribusi yang besar, karena memiliki alat-alat yang lebih matang untuk pengelolaan skala besar.
  - **Integrasi Semantik**: RDF mendukung integrasi semantik yang lebih baik, memungkinkan data dari berbagai sumber dapat dihubungkan dan dianalisis secara lebih mendalam.

#### 3. **Atomic Data vs GraphQL**

- **Kelebihan Atomic Data:**
  - **Auditabilitas & Versi**: Atomic Data menyediakan fitur versioning yang kuat dengan Atomic Commits, memungkinkan setiap perubahan disimpan sebagai transaksi yang dapat diaudit.
  - **Data Terhubung dan Terdesentralisasi**: Dengan menggunakan URL, Atomic Data memudahkan untuk menghubungkan dataset yang tersebar di berbagai sumber tanpa membuat duplikasi data.

- **Kelebihan GraphQL:**
  - **Kontrol Pengguna atas Data**: GraphQL memungkinkan klien menentukan secara spesifik data apa yang mereka inginkan dari server, mengurangi pengambilan data yang berlebihan dan meningkatkan efisiensi.
  - **Komunitas dan Ekosistem yang Lebih Besar**: GraphQL memiliki komunitas pengembang yang lebih luas dan berbagai alat bantu untuk mempermudah pengembangan API.
  - **Kinerja**: GraphQL lebih cepat dalam menangani query data yang kompleks karena hanya memerlukan pengambilan data yang diminta, tanpa memvalidasi tipe atau mengikuti skema ketat seperti Atomic Data.

## Kesimpulan

Atomic Data menawarkan fleksibilitas tinggi dalam pengelolaan data terstruktur dengan skema yang fleksibel, validasi tipe yang ketat, serta kemampuan audit dan versioning yang baik. Namun, untuk kasus penggunaan tertentu seperti skala besar, data internal, atau data multimedia, aplikasi lain seperti RDF, JSON-LD, dan GraphQL mungkin lebih tepat digunakan. Atomic Data unggul dalam kasus di mana interoperabilitas, auditabilitas, dan konektivitas data terdesentralisasi sangat dibutuhkan.


## Referensi

(https://docs.atomicdata.dev/)
