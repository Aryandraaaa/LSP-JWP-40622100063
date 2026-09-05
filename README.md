# LSP-JWP-40622100063
# Aplikasi To-Do List

Aplikasi sederhana berbasis **PHP** untuk mencatat dan mengelola tugas harian. Data tugas disimpan menggunakan **struktur data array** dan pendekatan **pemrograman terstruktur**, dengan tampilan antarmuka menggunakan **Bootstrap 5**.

## Deskripsi

Proyek ini merupakan aplikasi *To-Do List* berbasis web yang memungkinkan pengguna untuk menambah tugas, menandai tugas selesai, dan menghapus tugas. Seluruh data disimpan dalam *session* sehingga perubahan tetap tersimpan selama sesi browser aktif.

Aplikasi dibangun dengan:

- **PHP 8** — logika dan pemrosesan data
- **Bootstrap 5** — tampilan antarmuka responsif (via CDN)
- **Struktur data array of objects** — daftar tugas
- **Pemrograman terstruktur** — logika dibagi ke dalam fungsi-fungsi reusable

## Fitur

- **Tambah tugas** — menambahkan tugas baru melalui form input
- **Tandai tugas selesai** — mengubah status tugas dengan *checkbox*
- **Hapus tugas** — menghapus tugas dari daftar
- **Statistik tugas** — menampilkan jumlah total, selesai, dan belum selesai
- **Notifikasi aksi** — umpan balik berupa pesan *alert* untuk setiap aksi

## Struktur Folder

```
C:\xampp\htdocs\todolist/
├── index.php                # Halaman utama
├── includes/
│   ├── functions.php        # Logika aplikasi (fungsi CRUD & render)
│   ├── header.php           # Bagian awal layout (head + header)
│   └── footer.php           # Bagian akhir layout (footer + JS)
└── assets/
    └── css/
        └── style.css        # Gaya kustom aplikasi
```

### Keterangan file

| File | Fungsi |
|------|--------|
| `index.php` | Halaman utama; mengatur alur program (session, aksi, tampilan). |
| `includes/functions.php` | Berisi seluruh logika: `tambahTugas`, `ubahStatus`, `hapusTugas`, `tampilkanDaftar`, dll. |
| `includes/header.php` | Bagian atas layout: `<!DOCTYPE>`, `<head>`, dan header aplikasi. |
| `includes/footer.php` | Bagian bawah layout: penutup `<main>`, footer, dan skrip JS. |
| `assets/css/style.css` | Gaya kustom untuk mempercantik tampilan (melengkapi Bootstrap). |

## Cara Menjalankan

1. **Salin folder** proyek ini ke dalam `C:\xampp\htdocs\`.

   ```
   C:\xampp\htdocs\todolist\
   ```

2. **Jalankan XAMPP** dan pastikan layanan **Apache** dalam keadaan *Running*.

3. **Buka di browser** melalui alamat:

   ```
   http://localhost/todolist
   ```

### Prasyarat

- XAMPP (atau server web lain yang mendukung PHP) telah terpasang.
- Apache aktif pada port `80`.

## Teknologi yang Digunakan

- [PHP](https://www.php.net/) — bahasa pemrograman server-side
- [Bootstrap 5](https://getbootstrap.com/) — framework CSS (via CDN)
- [Bootstrap Icons](https://icons.getbootstrap.com/) — ikon antarmuka (via CDN)

## Kontributor

- [Aryandraaaa](https://github.com/Aryandraaaa)

---

> **Catatan:** Proyek ini dibuat untuk tujuan pembelajaran (tugas praktik). Silakan dikembangkan lebih lanjut — misalnya menyimpan data ke database (MySQL) atau menambahkan fitur pengeditan tugas.
