# EU Academy  
Learning Management System & Human Resource Management  

## Tujuan Proyek
Proyek **EU Academy** dikembangkan sebagai bagian dari **tugas mata kuliah Pemrograman Web Semester 4** yang dikerjakan secara bersama oleh mahasiswa mata kuliah Pemrograman Web kelas CR002.  
Pengembangan sistem ini bertujuan untuk menerapkan konsep pemrograman web secara komprehensif, mulai dari analisis kebutuhan, perancangan sistem, implementasi backend dan frontend, integrasi database, hingga pemanfaatan layanan eksternal.

## Deskripsi Proyek
EU Academy adalah aplikasi web terpadu untuk lembaga bimbingan belajar bahasa asing yang berfokus pada pengajaran Bahasa Inggris dan Bahasa Jepang bagi pemula. Sistem ini dirancang untuk mendukung proses bisnis utama EU Academy, mulai dari company profile, pengelolaan sumber daya manusia, pembelajaran berbasis LMS, hingga pembayaran online dan notifikasi otomatis.

Aplikasi ini dikembangkan berdasarkan dokumen **Business Requirement Document (BRD)** dan **Software Requirements Specification (SRS)** untuk memastikan kesesuaian antara kebutuhan bisnis dan implementasi teknis.

---

## Tujuan Pengembangan
- Menyediakan platform digital terpusat untuk pengelolaan pembelajaran dan administrasi
- Mempermudah proses pendaftaran peserta dan pembayaran course secara online
- Mendukung pengelolaan pengajar, absensi, gaji, dan cuti melalui sistem HRM
- Menyediakan LMS terstruktur dengan modul, quiz, penilaian, dan sertifikat digital
- Mengotomatisasi notifikasi melalui email dan WhatsApp

---

## Ruang Lingkup Sistem
Sistem EU Academy mencakup beberapa modul utama berikut:

### 1. Company Profile
- Home
- About Us
- Blog
- Contact Us  

### 2. HRM (Human Resource Management)
- Manajemen karyawan dan pengajar
- Departemen dan branch office
- Absensi pegawai dan pengajar
- Payroll (gaji karyawan dan pengajar)
- Manajemen cuti pengajar

### 3. LMS (Learning Management System)
- Event Course berbasis batch 6 bulan
- Jadwal pembelajaran offline (72 sesi)
- Modul pembelajaran dalam bentuk PDF
- Quiz sebagai tugas dan indikator kehadiran
- Penilaian dan rekap nilai
- Sertifikat digital kelulusan

### 4. Payment Gateway
- Integrasi Midtrans Sandbox
- Aktivasi otomatis akses LMS setelah pembayaran berhasil
- Verifikasi pembayaran melalui callback API

### 5. Notifikasi Otomatis
- Email (SMTP) untuk invoice pembayaran
- WhatsApp (Baileys) untuk ucapan selamat bergabung dan notifikasi akademik

---

## Karakteristik Pengguna
- **Admin Operasional Digital**
- **Tim Administrasi**
- **Tim Akademik**
- **Pengajar**
- **Peserta Didik**

Setiap pengguna memiliki hak akses berbasis **RBAC (Role-Based Access Control)**.

---

## Tech Stack
- **Backend**: Laravel 12
- **Frontend**: Livewire
- **Admin Panel**: Filament v3
- **Database**: MySQL
- **Payment Gateway**: Midtrans Sandbox
- **Notifikasi Email**: SMTP
- **Notifikasi WhatsApp**: Node.js, Express.js, Baileys
- **Containerization**: Docker
- **Web Server**: Nginx
- **Security Tunnel**: Cloudflare Zero Trust

---

## Fitur Utama
- CRUD Company Profile
- Manajemen HRM lengkap
- LMS terintegrasi dengan event course
- Pembayaran online dan verifikasi otomatis
- Pengiriman invoice dan notifikasi otomatis
- Penerbitan dan unduh sertifikat digital
- API internal untuk integrasi pembayaran dan notifikasi

---

## Kebutuhan Non-Fungsional
- Keamanan data dengan enkripsi dan HTTPS
- Autentikasi berbasis role
- Akses sistem 24/7
- Antarmuka user-friendly
- Sistem scalable dan portable menggunakan Docker
- Integrasi real-time dengan layanan eksternal

---

## Batasan Sistem
- Pembelajaran dilakukan secara offline
- Pembayaran hanya melalui Midtrans
- Materi pembelajaran hanya tersedia dalam bentuk digital