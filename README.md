# 🍷 Core Finance
*A Dark, Premium, and Intelligent Personal Finance Tracker*

[![Flutter Version](https://img.shields.io/badge/Flutter-3.12%2B-02569B?logo=flutter)](https://flutter.dev)
[![Dart Version](https://img.shields.io/badge/Dart-3.4%2B-0175C2?logo=dart)](https://dart.dev)
[![Version](https://img.shields.io/badge/Version-v1.5.0%20(Build%2010)-CC1B1B)](https://core-dev-group.my.id)
[![AI Powered](https://img.shields.io/badge/AI-Gemini%202.5%20Flash-D97706)](https://ai.google.dev/)
[![Storage](https://img.shields.io/badge/Storage-Hive%20%2B%20Firebase%20Cloud-FFCA28?logo=firebase)](https://firebase.google.com)
[![Powered By](https://img.shields.io/badge/Powered%20By-Core%20Dev%20Group-22C55E)](https://core-dev-group.my.id)

---

## 🌟 Tentang Proyek (*About The Project*)

**Core Finance** adalah aplikasi manajemen keuangan pribadi (*personal finance tracker*) bergaya gelap merah darah (*dark crimson glassmorphism*) yang menggabungkan kecepatan penyimpanan lokal **Hive NoSQL**, keandalan **Firebase Cloud Backup**, dan kecerdasan analitis dari **Core AI Advisor** berbasis **Gemini 2.5 Flash**.

Didesain untuk memberikan rasa kontrol penuh atas keuangan Anda dengan estetika kelas atas, animasi mulus, dan fitur esensial dari manajemen anggaran hingga ekspor kalender lokal HP.

---

## ✨ Fitur Unggulan — Mega Update v1.5.0

### 💰 1. Smart Budgeting & Alert Pengeluaran
- Atur batas pengeluaran bulanan per kategori (Makanan, Hiburan, Belanja, Transportasi, Tagihan, dll).
- Visualisasi progress bar dinamis yang menunjukkan persentase pemakaian anggaran.
- **Peringatan Otomatis (Alert):** Memberikan peringatan kuning ketika pengeluaran melampaui **80%** dan peringatan merah ketat ketika melampaui **100%**, terintegrasi langsung dengan saran **Core AI** dan halaman **Statistik**.

### 📑 2. Debt & Receivable Tracker (Pencatat Hutang & Piutang)
- Catat siapa yang berhutang kepada Anda (*Piutang*) dan kepada siapa Anda berhutang (*Hutang*).
- Indikator persentase pelunasan dan filter status (**Semua**, **Aktif**, **Lunas**).
- **Ekspor Jatuh Tempo ke Kalender HP:** Simpan tanggal jatuh tempo hutang dan piutang langsung ke kalender lokal ponsel dengan alarm pengingat otomatis (`VALARM`) 1 hari sebelumnya.

### 🧾 3. Split Bill & Kalkulator Patungan (*Fair Split Calculator*)
- Bagi tagihan nongkrong atau makan bersama dengan metode **Equal Split** (rata) atau **Custom Split** (disesuaikan per item/orang).
- Kalkulasi otomatis untuk penambahan **Pajak (Tax)** dan **Service Charge**.
- Simpan hasil perhitungan patungan langsung ke catatan pengeluaran harian hanya dalam satu ketukan.

### 🤖 4. Core AI Advisor & OCR Vision Scanner
- **Core AI Financial Advisor:** Asisten chat pintar berkarakter *Core AI* yang analitis, tenang, dan tegas. Memahami riwayat keuangan Anda secara presisi dengan konteks kronologi **Hari, Bulan, dan Tahun** yang akurat.
- **Vision Receipt Scanner:** Unggah foto atau jepret gambar struk belanja Anda, dan AI akan otomatis mengenali total transaksi, nama merchant, dan kategori untuk dicatat secara instan!

### 📅 5. Integrasi Kalender Lokal HP (`.ics / iCalendar Support`)
- Ekspor riwayat transaksi menjadi format standar internasional **`.ics` (RFC 5545)** yang mendukung penuh **Google Calendar**, **Apple Calendar**, **Outlook**, dan aplikasi kalender bawaan HP.
- Dukungan aturan perulangan (`RRULE:FREQ=DAILY/WEEKLY/MONTHLY/YEARLY`) untuk transaksi rutin serta alarm jatuh tempo.
- Akses ekspor cepat di 3 titik: Halaman **Export Data**, AppBar **Semua Transaksi**, dan AppBar **Hutang / Piutang**.

### 📤 6. Export Laporan Profesional (PDF & CSV)
- Generate laporan keuangan bergaya eksekutif dalam format **PDF** dan spreadsheet **CSV**.
- Dilengkapi ringkasan total pemasukan, pengeluaran, saldo bersih, serta tabel rincian transaksi lengkap.

### 📊 7. Pengelompokan Harian & Filter Kalender Lengkap
- Tampilan riwayat transaksi kini dikelompokkan secara kronologis harian (**Hari Ini**, **Kemarin**, dan tanggal lengkap seperti **4 Agustus 2026**).
- **Filter Rentang Waktu Dasbor:** Chip filter cepat untuk *Semua*, *Hari Ini*, *Kemarin*, *7 Hari*, *30 Hari*, *Bulan Ini*, serta tombol **Kalender**.
- **Filter Lihat Semua Transaksi:** Saring riwayat berdasarkan **Tahun**, **Bulan**, dan **Tanggal** khusus dengan tombol **Reset** cepat.

### ☁️ 8. Cloud Backup & Restore (Firebase)
- Backup dan restore data secara aman ke **Firebase Cloud Firestore** yang dikaitkan dengan akun pengguna (Google Sign-In).
- Mendukung **Mode Guest**: Pengguna dapat masuk dan menggunakan aplikasi secara offline, dan akan menerima pemberitahuan ramah jika ingin mengaktifkan backup awan.

### 🌐 9. Multi-Bahasa & Multi-Mata Uang Internasional
- **6 Bahasa Resmi:** Indonesia (ID), English (EN), Bahasa Melayu (MS), العربية (AR), 中文 (ZH), 日本語 (JA).
- **6 Mata Uang:** IDR (Rp), USD ($), MYR (RM), SAR (﷼), CNY (¥), JPY (¥).
- Format angka, simbol, dan tanggal otomatis menyesuaikan dengan preferensi lokal Anda.

---

## 📱 Arsitektur & Teknologi

| Komponen | Teknologi yang Digunakan |
| :--- | :--- |
| **Framework** | Flutter 3.x & Dart 3.x |
| **State Management** | `provider` (MultiProvider Reactive State) |
| **Local Storage** | `hive` & `hive_flutter` (Zero-latency NoSQL Key-Value Store) |
| **Cloud Service** | `firebase_core`, `firebase_auth`, `cloud_firestore`, `google_sign_in` |
| **AI & NLP Engine** | `Gemini 2.5 Flash` via Google Gemini API |
| **OCR Vision Engine** | `Gemini 2.5 Flash` via Google Gemini API |
| **Export Engine** | `pdf`, `csv`, `path_provider`, `share_plus` |
| **Calendar Standard** | RFC 5545 `.ics` Generator (`VALARM`, `RRULE`) |
| **Typography & UI** | `google_fonts` (Inter), Custom Dark Crimson Glassmorphism |

---

## 🚀 Cara Instalasi & Menjalankan Aplikasi (*Getting Started*)

### 1. Prasyarat (*Prerequisites*)
Pastikan Anda telah menginstal lingkungan pengembangan Flutter di sistem Anda:
- **Flutter SDK:** `>= 3.12.0`
- **Dart SDK:** `>= 3.4.0`
- **Android Studio / VS Code / Xcode** (untuk target mobile atau desktop)

### 2. Langkah Instalasi
```bash
# 1. Clone repositori ini ke dalam direktori lokal Anda
git clone https://github.com/kodel-dev/finance-makima.git
cd finance-makima

# 2. Unduh dan instal seluruh dependensi paket Dart & Flutter
flutter pub get

# 3. Jalankan pemeriksaan linter / static analysis (opsional, untuk memastikan kode bersih)
flutter analyze

# 4. Jalankan aplikasi di emulator atau perangkat fisik yang terhubung
flutter run
```

### 3. Konfigurasi Khusus (Opsional)
- **Gemini API Key:** Untuk menggunakan fitur Core AI Advisor dan Receipt Scanner, Anda harus mengatur API Key dari Google AI Studio melalui menu Pengaturan Profil di dalam aplikasi.
- **Firebase:** Proyek ini menggunakan konfigurasi default `nam5 (United States)`. Anda dapat menimpa `google-services.json` (Android) atau `GoogleService-Info.plist` (iOS) dengan proyek Firebase Anda sendiri jika ingin melakukan self-hosting backend.

---

## 📁 Struktur Direktori (*Folder Structure*)

```text
lib/
 ├── l10n/
 │    └── app_strings.dart          # Kamus multi-bahasa (ID, EN, MS, AR, ZH, JA)
 ├── models/
 │    ├── budget.dart               # Model anggaran tahunan/bulanan per kategori
 │    ├── debt.dart                 # Model pencatat hutang dan piutang
 │    ├── profile.dart              # Model profil pengguna dan preferensi
 │    └── transaction.dart          # Model transaksi harian (Favorit, Berulang, dll)
 ├── providers/
 │    ├── budget_provider.dart      # CRUD anggaran dan kalkulasi progress pemakaian
 │    ├── currency_provider.dart    # Pengelola preferensi mata uang (IDR, USD, dll)
 │    ├── debt_provider.dart        # CRUD hutang/piutang dan perhitungan pelunasan
 │    ├── locale_provider.dart      # Pengelola perubahan bahasa secara instan
 │    ├── profile_provider.dart     # Pengelola akun dan gambar profil pengguna
 │    └── transaction_provider.dart # Pengelola transaksi utama & auto-generate recurring
 ├── screens/
 │    ├── dashboard/                # Komponen kartu dasbor (Header, Saldo, Recent)
 │    ├── profile/                  # Komponen modal pemilih bahasa & mata uang
 │    ├── add_transaction_screen.dart # Layar tambah transaksi + filter Favorit/Berulang
 │    ├── all_transactions_screen.dart # Layar semua transaksi + filter Kalender/Hari/Bulan
 │    ├── budget_screen.dart        # Layar kelola anggaran dan indikator alert merah/kuning
 │    ├── debt_screen.dart          # Layar kelola hutang/piutang + ekspor ke kalender HP
 │    ├── edit_transaction_screen.dart # Layar sunting transaksi
 │    ├── export_screen.dart        # Layar ekspor laporan PDF, CSV, dan Kalender .ics
 │    ├── login_screen.dart         # Layar masuk akun Google / Mode Guest
 │    ├── main_screen.dart          # Navigasi utama (Bottom Navigation Bar)
 │    ├── profile_screen.dart       # Layar profil, menu versi APK, & pengaturan backup
 │    ├── recurring_screen.dart     # Layar daftar transaksi berulang otomatis
 │    ├── split_bill_screen.dart    # Layar kalkulator patungan & pembagian tagihan
 │    └── statistics_screen.dart    # Layar grafik statistik pengeluaran/pemasukan
 ├── services/
 │    ├── ai_service.dart           # Layanan Core AI Chat & Scanner Struk Vision
 │    ├── app_version_service.dart  # Layanan informasi versi APK & modal dialog tentang
 │    ├── backup_service.dart       # Layanan sinkronisasi Firebase Cloud Firestore
 │    ├── calendar_service.dart     # Generator file kalender iCalendar (.ics / RFC 5545)
 │    └── export_service.dart       # Generator laporan dokumen PDF dan CSV
 ├── theme/
 │    └── app_theme.dart            # Sistem warna Dark Crimson, glassmorphism, & Google Fonts
 └── main.dart                      # Titik masuk utama aplikasi & inisialisasi Hive/Firebase
```

---

## 💡 Tips Penggunaan (*Pro Tips*)

1. **Gunakan Mode Guest Secara Bebas:** Anda dapat langsung mencatat transaksi saat pertama kali membuka aplikasi tanpa perlu login. Jika Anda menekan tombol *Backup Cloud* dalam mode guest, aplikasi akan memberi tahu secara ramah bahwa Anda perlu login terlebih dahulu.
2. **Pindai Struk dengan Core AI:** Pada layar Dasbor atau ruang obrolan AI, ketuk ikon kamera/gambar untuk memindai struk restoran atau belanjaan. AI akan langsung menyimpulkan nominal dan kategori untuk Anda.
3. **Impor ke Kalender Ponsel:** Pada menu **Export Data**, pilih **"Export ke Kalender HP (.ics)"**. File kalender standar akan dibuat dan langsung dapat dibuka dengan Google Calendar atau Apple Calendar Anda!
4. **Pantau Versi Aplikasi:** Ketuk baris menu **Versi** di halaman **Profil** atau badge di footer untuk melihat status build dan menyalin informasi spesifikasi aplikasi dengan mudah.

---

## 👥 Kredit & Kontributor (*Credits & Attribution*)

- **Developed & Powered by:** [Core Dev Group](https://core-dev-group.my.id)
- **App Edition:** *v1.5.0 (Build 10)*
- **AI Backend:** Powered by [Google Gemini API](https://ai.google.dev/).
- **License:** MIT License — bebas digunakan dan dimodifikasi untuk tujuan pengembangan non-komersial dan komersial sesuai ketentuan lisensi.

---
*“Pegang kendali atas keuanganmu, sebelum keuanganmu yang mengendalikanmu.”* — **Core Finance** 🍷
