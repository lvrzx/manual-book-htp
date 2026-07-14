# 📘 Manual Book — Chatbot HTP Indonesia

Panduan interaktif untuk chatbot AI Customer Service, pendaftaran otomatis, dan follow-up pendaftar HTP Indonesia. Dibuat sebagai halaman web satu-file (HTML), lengkap dengan simulasi percakapan Telegram dan animasi alur kerja.

🔗 **Lihat langsung:** https://lvrzx.github.io/manual-book-htp/

## Isi Manual Book

- **Cara Kerja Sistem** — gambaran 3 alur otomatis (chatbot, otomatisasi pendaftaran, follow-up)
- **Panduan Calon Siswa** — langkah demi langkah pakai chatbot, dari `/start` sampai pendaftaran berhasil
- **Panduan Admin** — jenis notifikasi, arti status pendaftar di Google Sheets, cara kelola Knowledge Base
- **Troubleshooting** — solusi masalah teknis yang umum terjadi

## Untuk Siapa

- **Calon siswa** — belajar cara chat dan mendaftar lewat bot Telegram HTP Indonesia
- **Admin/tim HTP Indonesia** — memahami alur notifikasi, status pendaftar, dan cara menjaga sistem tetap jalan

## Struktur Proyek

```
manual-book-htp/
├── index.html   # halaman manual book (satu file, tanpa dependensi eksternal selain Google Fonts)
└── README.md    # dokumen ini
```

## Menjalankan/Mengedit Secara Lokal

Tidak perlu instalasi apa pun — cukup buka `index.html` langsung di browser, atau jalankan server lokal sederhana:

```bash
python3 -m http.server 8000
```

lalu buka `http://localhost:8000` di browser.

## Update Konten

Semua teks, warna, dan animasi ada langsung di dalam `index.html` (CSS & JavaScript inline). Untuk memperbarui isi:

1. Edit bagian yang relevan di `index.html` (section `Panduan Calon Siswa`, `Panduan Admin`, dll).
2. Commit & push perubahan ke branch `main`.
3. GitHub Pages otomatis memperbarui halaman dalam 1–2 menit.

## Terkait

Halaman ini menjelaskan tiga workflow n8n milik HTP Indonesia:

| Workflow | Fungsi |
|---|---|
| WF1 — Chatbot AI Customer Service | Menjawab pertanyaan calon siswa & mengarahkan ke pendaftaran |
| WF2 — Otomatisasi Data Pendaftaran | Validasi & simpan data pendaftar ke Google Sheets |
| WF3 — Follow-Up Pendaftar | Pengingat berjenjang otomatis + laporan harian ke admin |

---
© HTP Indonesia — Lembaga Kursus & Pelatihan Komputer Terpercaya
