# Deploy website Puspa Miauw

Website statis murni (HTML saja, tanpa build, tanpa server). Foto sudah tertanam di `index.html`.

## Isi folder
- `index.html` : halaman utama (wajib)
- `favicon.svg` : ikon tab browser
- `404.html` : halaman error (dipakai GitHub Pages dan sebagian hosting)
- `robots.txt` : izin mesin pencari
- `.nojekyll` : agar GitHub Pages tidak memproses file

## Sebelum upload
Buka `index.html` dengan editor teks, cari blok `CONFIG` dekat akhir file, lalu ganti email (dan isi nomor WhatsApp jika mau, format `6281234567890`).

## Hostinger / IDwebhost / cPanel
1. Masuk File Manager, buka folder `public_html`.
2. Upload semua isi folder Deploy (bukan folder Deploy-nya), termasuk `.nojekyll` jika terlihat.
3. Buka domain Anda. `index.html` otomatis tampil.

## GitHub Pages
1. Buat repository baru, upload semua isi folder Deploy ke branch `main`.
2. Settings > Pages > Source: Deploy from a branch > `main` / `(root)` > Save.
3. Situs aktif di `https://<username>.github.io/<repo>/` dalam beberapa menit.

## Netlify / Cloudflare Pages / Vercel
Drag and drop folder Deploy ke dashboard, tanpa build command, publish directory kosong atau `/`.
