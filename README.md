# CLASS ASSISTANT — Premium Static

Project website kelas yang siap deploy ke Vercel.

## Struktur
- `index.html` — halaman utama
- `style.css` — seluruh desain
- `script.js` — fungsi/interaksi
- `data/class.json` — **rename identitas aplikasi/kelas di sini**
- `data/students.json` — database siswa
- `data/schedule.json` — database jadwal
- `data/duty.json` — database piket
- `data/tasks.json` — database tugas awal
- `data/cash.json` — database kas awal
- `data/announcements.json` — database pengumuman awal
- `assets/` — tempat logo/gambar tambahan

## Cara rename paling mudah
Buka `data/class.json`, lalu ubah:
- `appName`
- `className`
- `schoolName`
- `schoolYear`
- `homeroomTeacher`
- `classLeader`

Untuk mengganti isi database, edit file JSON masing-masing.

## Deploy Vercel
Upload/import seluruh folder project. Jangan hanya upload `index.html`; folder `data` harus ikut karena website membaca JSON menggunakan `fetch()`.

Framework: Other / Static.
Build command: kosong.
Output directory: `.`

## Catatan database
JSON di dalam project adalah **database statis** untuk data awal. Tambah data dari halaman akan bekerja selama halaman sedang terbuka, tetapi perubahan tersebut tidak menulis kembali ke file JSON di server. Untuk database online yang permanen, nanti bisa dihubungkan ke Supabase/Firebase.
