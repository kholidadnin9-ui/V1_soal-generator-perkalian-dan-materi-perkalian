# Soal Generator Perkalian dan Materi Perkalian

Media pembelajaran interaktif perkalian 1–10 untuk siswa kelas 2 SD. Aplikasi dibuat menggunakan React, TypeScript, dan Vite.

## Menjalankan secara lokal

Persyaratan: Node.js 22 atau versi LTS yang kompatibel dan npm.

```bash
npm ci
npm run dev
```

## Build dan pratinjau produksi

```bash
npm run build
npm run preview
```

Hasil build tersedia di folder `dist/`.

## Pengujian

```bash
npm run typecheck
npm test
```

Tes browser menggunakan Playwright. Jika browser Chromium belum terpasang, jalankan `npx playwright install chromium` terlebih dahulu.

## Hosting di GitHub Pages

1. Buat repositori GitHub dengan nama **`soal-generator-perkalian-dan-materi-perkalian`**. Nama repositori sebaiknya tanpa spasi.
2. Unggah seluruh isi folder proyek ke branch `main` (pastikan `package.json`, `package-lock.json`, `index.html`, `src/`, `public/`, dan `.github/` berada di root repositori). Jangan unggah `node_modules/` atau `dist/`.
3. Buka **Settings → Pages** pada repositori. Di bagian **Build and deployment**, pilih **GitHub Actions** sebagai Source.
4. Buka tab **Actions**, lalu tunggu workflow **Deploy to GitHub Pages** selesai dengan status berhasil.
5. Situs akan tersedia di `https://USERNAME.github.io/soal-generator-perkalian-dan-materi-perkalian/` setelah workflow berhasil. Ganti `USERNAME` dengan nama pengguna GitHub Anda.

### Jika nama repositori diubah

Perbarui opsi `base` di `vite.config.ts` agar sama persis dengan nama repositori, dengan garis miring di awal dan akhir, lalu commit perubahan.

## Catatan

Gambar pembelajaran disimpan secara lokal di `public/images/`. URL gambar memakai `import.meta.env.BASE_URL` agar sesuai dengan jalur GitHub Pages.
