# Lab Fotografi (aplikasi web)

Aplikasi belajar fotografi dengan tiga tab: Segitiga Exposure, Lensa dan Jarak, Cahaya Studio 3D.
Bisa dipasang di layar utama HP dan tetap jalan tanpa internet setelah dibuka sekali.

## Isi folder
- `index.html` — aplikasinya
- `manifest.webmanifest` — nama, ikon, dan warna aplikasi
- `sw.js` — menyimpan aplikasi supaya bisa dibuka offline
- `icon-*.png`, `icon.svg` — ikon aplikasi

## Cara mempublikasikan (pilih salah satu, semua gratis)
Aplikasi harus dibuka lewat alamat **https** supaya bisa dipasang dan jalan offline.

1. **Netlify Drop** (paling mudah): buka app.netlify.com/drop, lalu seret folder ini ke halaman itu. Kamu langsung dapat alamat https.
2. **Cloudflare Pages**: Workers & Pages → Create → Pages → Upload assets → unggah folder ini.
3. **GitHub Pages**: unggah isi folder ke repositori, lalu aktifkan Pages di Settings.

Semua file harus berada di folder yang sama. Jangan ganti nama file.

## Cara memasang di HP
- **Android (Chrome)**: buka alamatnya, ketuk tombol **Pasang** di bagian atas, atau menu ⋮ → *Instal aplikasi*.
- **iPhone (Safari)**: buka alamatnya, ketuk **Bagikan** → *Tambah ke Layar Utama*.

## Memperbarui aplikasi
Setelah mengganti `index.html`, ubah juga baris pertama `sw.js` (misalnya `lab-foto-v1` menjadi `lab-foto-v2`), lalu unggah ulang. HP murid akan mengambil versi baru saat aplikasi dibuka dengan internet.

## Catatan
- Huruf (font) diambil dari Google Fonts saat pertama online. Kalau offline sebelum sempat tersimpan, aplikasi memakai huruf bawaan HP. Isinya tetap sama.
- Tab Lensa dan Cahaya Studio 3D memakai WebGL. HP keluaran beberapa tahun terakhir mendukungnya.
- Membuka `index.html` langsung dari file (tanpa hosting) tetap bisa dipakai, tapi tidak bisa dipasang dan tidak offline.
