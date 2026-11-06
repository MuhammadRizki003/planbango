# Viewer 3D Proyek

Web sederhana untuk menampilkan model SketchUp (diekspor ke .glb) lewat GitHub Pages.

## Struktur
- `index.html` : halaman utama, daftar gambar + tombol "Lihat 3D"
- `viewer.html` : halaman viewer 3D, tombol "Kembali" ke halaman utama
- `models.js` : DAFTAR gambar (edit di sini)
- `models/` : taruh file .glb di sini
- `thumbs/` : (opsional) gambar thumbnail
- `style.css` : tampilan

## Mengganti placeholder dengan model asli
1. Ekspor dari SketchUp ke .glb.
2. Timpa file di `models/` dengan nama sama (mis. `lantai-1.glb`), atau ubah `file:` di `models.js`.

## Menambah gambar baru
Salin satu blok di `models.js`, ubah `id` (unik, tanpa spasi), `title`, `desc`, `file`.

## Aktifkan GitHub Pages
Settings → Pages → Deploy from a branch → `main` → `/ (root)` → Save.

Catatan: jangan buka lewat klik dua kali (file://) karena model tidak akan termuat; gunakan GitHub Pages
atau server lokal (`python -m http.server`).
