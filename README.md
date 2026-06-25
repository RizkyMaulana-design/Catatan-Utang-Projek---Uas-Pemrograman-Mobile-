# CatatanUtang

CatatanUtang adalah aplikasi Android untuk membantu pemilik warung, toko kecil, atau usaha harian dalam mencatat hutang pelanggan secara cepat, rapi, dan mudah dipantau. Aplikasi ini dirancang agar proses pencatatan hutang tidak lagi bergantung pada buku manual, sehingga pemilik usaha bisa melihat data pelanggan, total piutang, transaksi hutang, dan pembayaran dari satu dashboard yang sederhana.

## Status Project

Status pengembangan: **Final Release**

Project ini sudah mencapai **tahapan akhir** dan sudah **ready 100%** untuk digunakan sebagai aplikasi pencatatan hutang pelanggan berbasis Android. Seluruh fitur utama yang dibutuhkan untuk alur pencatatan hutang sudah tersedia, mulai dari dashboard, tambah pelanggan, catat transaksi, tambah hutang, terima pembayaran, sampai pembaruan total piutang secara otomatis.

## Tampilan Aplikasi

<img width="300" alt="Menu Dashboard" src="https://github.com/user-attachments/assets/e11e612b-c77d-4582-8267-8f4f1d905d74" />

<img width="300"  alt="formulir Pendaftaran" src="https://github.com/user-attachments/assets/c4238c95-7b52-44e8-9a18-f38bda412fa1" />

## Deskripsi Singkat

Aplikasi ini dibuat untuk mempermudah pemilik usaha dalam mengelola hutang pelanggan. Pengguna dapat menambahkan pelanggan baru, mencatat nominal hutang, menerima pembayaran, dan melihat perubahan total piutang secara langsung di dashboard.

CatatanUtang cocok digunakan untuk:

- Warung sembako
- Toko kelontong
- Usaha rumahan
- Penjual harian
- UMKM yang membutuhkan pencatatan piutang sederhana

## Fitur Utama

- Dashboard utama untuk melihat ringkasan total piutang.
- Tampilan sambutan pengguna yang lebih ramah dan profesional.
- Ringkasan hutang jatuh tempo minggu ini.
- Tambah pelanggan baru dengan data penting seperti nama, nomor WhatsApp, alamat, dan nominal awal.
- Catat transaksi pelanggan secara langsung dari menu dashboard.
- Pilih pelanggan melalui dropdown.
- Input pelanggan tetap bisa diketik manual.
- Fitur Tambah Hutang untuk menambah saldo hutang pelanggan.
- Fitur Terima Pembayaran untuk mengurangi saldo hutang pelanggan.
- Total piutang di dashboard otomatis berubah setelah transaksi berhasil disimpan.
- Daftar pelanggan menampilkan data pelanggan dan sisa hutang terbaru.
- Profil pengguna dengan inisial dan foto profil.
- Dukungan deteksi lokasi untuk kebutuhan pencatatan berbasis lokasi.
- Desain antarmuka bersih, modern, dan mudah digunakan.
- Data disimpan secara lokal menggunakan SharedPreferences.

## Alur Penggunaan Aplikasi

1. Pengguna membuka aplikasi.
2. Aplikasi menampilkan halaman awal dan masuk ke dashboard.
3. Pengguna dapat melihat total piutang saat ini.
4. Pengguna menambahkan pelanggan baru melalui tombol tambah.
5. Data pelanggan disimpan ke penyimpanan lokal aplikasi.
6. Saat pelanggan ingin berhutang lagi, pengguna masuk ke menu Catat Transaksi.
7. Pengguna memilih pelanggan dari dropdown atau mengetik nama pelanggan.
8. Pengguna memilih tipe transaksi Tambah Hutang.
9. Nominal hutang dimasukkan dan dikonfirmasi.
10. Saldo hutang pelanggan bertambah.
11. Saat pelanggan membayar, pengguna memilih tipe transaksi Terima Pembayaran.
12. Nominal pembayaran dimasukkan dan dikonfirmasi.
13. Saldo hutang pelanggan berkurang.
14. Dashboard otomatis menampilkan total piutang terbaru.

## Detail Fitur Transaksi

### Tambah Hutang

Fitur ini digunakan ketika pelanggan ingin menambah hutang. Pengguna cukup memilih pelanggan, memasukkan nominal, memilih tanggal transaksi, lalu menekan tombol konfirmasi. Setelah transaksi berhasil, saldo hutang pelanggan akan bertambah dan total piutang pada dashboard ikut diperbarui.

### Terima Pembayaran

Fitur ini digunakan ketika pelanggan membayar sebagian atau seluruh hutangnya. Pengguna memilih pelanggan, memasukkan nominal pembayaran, lalu mengonfirmasi transaksi. Setelah berhasil, saldo hutang pelanggan akan berkurang dan dashboard menampilkan total piutang terbaru.

## Teknologi yang Digunakan

- Kotlin
- Android Native Views
- XML Layout
- SharedPreferences
- Material Components
- Gradle Kotlin DSL
- Android Studio

## Struktur Project

```text
CatatanUtang/
+-- app/
|   +-- src/main/
|       +-- java/com/example/catatanutang/
|       +-- res/
+-- docs/
|   +-- screenshots/
+-- gradle/
+-- build.gradle.kts
+-- settings.gradle.kts
+-- gradlew
+-- gradlew.bat
```

## Halaman Aplikasi

- Splash Screen
- Halaman izin lokasi
- Login
- Register
- Lupa password
- Dashboard
- Tambah pelanggan
- Daftar pelanggan
- Catat transaksi
- Profil pengguna

## Penyimpanan Data

Data aplikasi disimpan secara lokal menggunakan SharedPreferences. Data yang disimpan meliputi:

- Nama pengguna
- Inisial pengguna
- Foto profil
- Daftar pelanggan
- Nomor WhatsApp pelanggan
- Alamat pelanggan
- Limit atau nominal hutang awal
- Sisa hutang pelanggan
- Total piutang
- Total hutang jatuh tempo

## Cara Menjalankan Project

1. Clone repository ini.
2. Buka project menggunakan Android Studio.
3. Pastikan Android Studio sudah menggunakan JDK minimal Java 11.
4. Tunggu proses Gradle Sync selesai.
5. Jalankan aplikasi ke emulator atau perangkat Android.

Build melalui terminal:

```bash
./gradlew assembleDebug
```

Build melalui Windows PowerShell:

```powershell
.\gradlew.bat assembleDebug
```

APK debug akan tersedia di:

```text
app/build/outputs/apk/debug/app-debug.apk
```

## Kebutuhan Sistem

- Android Studio versi terbaru
- JDK 11 atau lebih baru
- Android SDK
- Perangkat Android atau emulator
- Minimum SDK: 29
- Target SDK: 36

## Keunggulan Aplikasi

- Mudah digunakan oleh pemilik usaha kecil.
- Tidak membutuhkan server untuk penggunaan dasar.
- Data transaksi langsung mempengaruhi dashboard.
- Tampilan sederhana dan tidak membingungkan.
- Cocok untuk pencatatan hutang harian.
- Bisa digunakan sebagai dasar pengembangan aplikasi UMKM yang lebih besar.

## Status Kesiapan

Project ini sudah **selesai 100%** untuk kebutuhan utama pencatatan hutang pelanggan.

Fitur yang sudah siap:

- Dashboard siap digunakan.
- Tambah pelanggan siap digunakan.
- Catat transaksi siap digunakan.
- Tambah hutang siap digunakan.
- Terima pembayaran siap digunakan.
- Update total piutang otomatis siap digunakan.
- Daftar pelanggan siap digunakan.
- Profil pengguna siap digunakan.
- Tampilan aplikasi siap digunakan.

## Catatan Rilis

Versi saat ini sudah berada pada tahap akhir pengembangan. Aplikasi sudah bisa dijalankan, diuji, dan digunakan sebagai aplikasi pencatatan hutang pelanggan berbasis Android.

## Lisensi

Project ini dibuat untuk kebutuhan pembelajaran, portofolio, dan pengembangan aplikasi pencatatan hutang sederhana.
