# NoteStation
Sebuah web atau platform berbagi catatan yang memungkinkan pengguna membuat, menyimpan, dan mengorganisasi berbagai jenis catatan secara digital. Layanan ini mendukung penulisan catatan dalam format text, penyisipan lampiran seperti gambar dan dokumen, serta pengelompokan catatan ke dalam berbagai kategori. Dengan kombinasi fitur pencatatan, Note Station menjadi solusi lengkap untuk menyimpan dan mengelola informasi secara terstruktur dan aman.

![Screenshot_16-12-2025_212531_notestation up railway app](https://github.com/user-attachments/assets/e21cf351-a9f2-4a6d-a98c-ee5f9068c76b)

## Fitur

### Manajemen Catatan
- **Rich Text Editor**: Editor WYSIWYG lengkap dengan TipTap yang mendukung:
  - Format teks (bold, italic, underline, headings)
  - List, tabel, dan code blocks
  - Upload gambar dengan kemampuan resize
  - Lampiran file (PDF, gambar, dokumen)
  - Syntax highlighting untuk kode
- **Auto-save**: Penyimpanan otomatis draft untuk mencegah kehilangan data
- **Tags & Kategori**: Organisasi catatan dengan tag kustom
- **Kontrol Visibilitas**: Berbagi catatan publik, private, atau khusus universitas
- **Manajemen File**: Upload dan kelola lampiran dengan ekstraksi teks PDF

### Fitur Berbasis AI
- **NORA AI (Note Research Assistant)**: Interface chat interaktif untuk pertanyaan terkait catatan
- **Ringkasan Otomatis**: Ringkasan catatan yang dibuat AI
- **Pembuatan Flashcard**: Buat flashcard belajar otomatis dari catatan

### Fitur Sosial
- **Bookmarking**: Simpan catatan favorit untuk akses cepat
- **Sistem Like**: Berinteraksi dengan konten komunitas
- **Leaderboard**: Berkompetisi dengan teman berdasarkan kontribusi
- **Pelacakan Aktivitas**: Monitor streak belajar dan progres mingguan
- **Profil Pengguna**: Profil yang dapat dikustomisasi dengan informasi universitas dan program studi

## Tech Stack

### Backend
- **Framework**: Laravel 12.0 (PHP 8.4)
- **Autentikasi**: Laravel Fortify
- **Storage**: AWS S3 (via Supabase)
- **Sistem Queue**: Database-based queues untuk background jobs

### Frontend
- **UI Framework**: React 19.2
- **Routing**: Inertia.js + Laravel Wayfinder
- **Editor**: TipTap
- **Styling**: Tailwind CSS
- **Komponen UI**: Radix UI + shadcn/ui
- **Icons**: Lucide React
- **Build Tool**: Vite 7.0
- **Type Safety**: TypeScript 5.7

### Database
- PostgreSQL (via Supabase)

### AI
- Groq AI

## Persyaratan

- PHP >= 8.4
- Composer
- Node.js >= 18
- PostgreSQL
- AWS S3 bucket (untuk penyimpanan file)

## Cara Penggunaan

### Membuat Catatan
1. Login ke akun Anda
2. Navigasi ke "Tambah Catatan"
3. Gunakan rich text editor untuk menulis catatan
4. Tambahkan tag dan atur visibilitas
5. Upload lampiran jika diperlukan
6. Simpan atau publish catatan Anda

### AI Integration
1. **Generate Summary dan Flashcard**: Klik "Generate Flashcard" pada pengaturan catatan
2. **NORA AI Chat**: Tanyakan pertanyaan tentang catatan Anda kepada NORA

### Bookmarking
- Klik ikon bookmark untuk menyimpan catatan
- Like catatan untuk menunjukkan apresiasi
- Lihat catatan yang di-bookmark di profil Anda

### Leaderboard
- Lihat kontributor teratas dalam kampus/prodi Anda
- Filter berdasarkan prodi, universitas atau peringkat global
- Berkompetisi berdasarkan pembuatan catatan dan engagement

### Badges
- Berisi 40++ badges yang bisa diperoleh pengguna
- Terdapat berbagai kategori lencana (ContentCreator, Engagement, Bookmarks, Community, Leaderboard, Streak, University Pride, Special)

## Acknowledgments

- Dibangun dengan [Laravel](https://laravel.com)
- Didukung oleh [React](https://react.dev)
- Komponen UI dari [Radix UI](https://www.radix-ui.com/)
- Icons oleh [Lucide](https://lucide.dev)
- Rich text editing via [TipTap](https://tiptap.dev)
