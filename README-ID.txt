# Nto.presett Web Patcher — Vercel

## Isi
- `website/index.html`: halaman web utama.
- `vercel.json`: mengarahkan URL utama `/` ke `/website/index.html`.

## Deploy lewat GitHub (disarankan)
1. Ekstrak ZIP ini di komputer/HP.
2. Buat repository baru di https://github.com/new lalu upload seluruh isi folder ini (`website/` dan `vercel.json`).
3. Buka https://vercel.com/new dan masuk dengan GitHub.
4. Import repository yang baru dibuat.
5. Framework Preset: pilih `Other`.
6. Build Command: kosongkan / matikan `Override` jika tersedia.
7. Output Directory: kosongkan / default; tidak perlu build.
8. Klik **Deploy**. Setelah selesai, buka domain `.vercel.app` yang diberikan.

## Catatan penting
Halaman ini tetap menggunakan API eksternal yang sudah tertanam di kode:
`https://api.kuronaiapp.com`
Vercel hanya meng-host halaman HTML; Vercel tidak otomatis meng-host API pemrosesan video tersebut. Fitur pemrosesan akan bekerja hanya jika API masih aktif, mengizinkan request dari domain Vercel (CORS), dan endpoint-nya tetap kompatibel. Jika muncul error CORS/API/akses ditolak, perbaikannya perlu dilakukan di server API oleh pemiliknya.

File ini adalah website statis, bukan lagi ekstensi browser yang dapat memodifikasi halaman TikTok secara langsung.
