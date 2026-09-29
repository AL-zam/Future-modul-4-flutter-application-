# flutter_application_1

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Learn Flutter](https://docs.flutter.dev/get-started/learn-flutter)
- [Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Flutter learning resources](https://docs.flutter.dev/reference/learning-resources)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.




# Portal Pengumuman TRPL (Modul 04 - REST API & Riverpod)

Aplikasi Flutter untuk menampilkan daftar pengumuman kampus secara *real-time* dari server melalui REST API. Project ini menggunakan **Riverpod** sebagai *state management* serta menerapkan pola penanganan kondisi asinkron (*4-State Pattern: Loading, Error, Empty, Success*).

---

##  Fitur Utama

* **Integrasi REST API**: Mengambil data pengumuman secara *asynchronous* dari server backend.
* **State Management (Riverpod)**: Pengelolaan data dinamis menggunakan `flutter_riverpod` (`FutureProvider` & `StateProvider`).
* **Filter Kategori**: Menyaring daftar pengumuman berdasarkan kategori (*Semua, Akademik, Beasiswa, Kegiatan, Prestasi*).
* **Penanganan 4-State UI**:
  *  **Loading State**: Indikator *loading* saat data sedang diunduh.
  *  **Error State**: Tampilan pesan error interaktif dilengkapi tombol *Coba Lagi* (*Retry*).
  *  **Empty State**: Informasi khusus jika data pada kategori yang dipilih kosong.
  *  **Success State**: Menampilkan daftar pengumuman lengkap dengan dukungan fitur *Pull-to-Refresh*.
* **Halaman Detail**: Menampilkan rincian isi pengumuman, penulis, tanggal rilis, dan statistik jumlah pembaca.

---

##  Library

* **Framework**: [Flutter](https://flutter.dev) (Dart SDK)
* **State Management**: [`flutter_riverpod`](https://pub.dev/packages/flutter_riverpod)
* **HTTP Client**: [`http`](https://pub.dev/packages/http)

---
