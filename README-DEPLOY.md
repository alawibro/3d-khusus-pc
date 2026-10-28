# Biodata + Stage 3D Bintang Zero (versi PC/laptop)

Versi ini khusus layar laptop/desktop. Dua model dipakai: Bintang Zero dan Radler Lemon, keduanya GLB asli tanpa kompresi (32,7 MB dan 27,3 MB). Pilih varian lewat tombol di bawah stage. Muatnya lebih lama dari versi universal, tetapi kualitasnya penuh.

## Deploy ke GitHub Pages

1. Buat repository baru di GitHub, misalnya `biodata`.
2. Unggah **isi** folder ini ke root repository: `index.html`, `css/`, `js/`, `assets/`, dan `README-DEPLOY.md`.
3. Buka **Settings → Pages**.
4. Di bagian **Build and deployment**, pilih **Deploy from a branch**. Pilih branch `main` dan folder `/ (root)`, lalu Save.
5. Tunggu beberapa menit. Situs tersedia di `https://<username>.github.io/<nama-repo>/`.

Catatan:
- `assets/3d/bintang-1.glb` berukuran 32,7 MB. GitHub memberi peringatan di atas 50 MB dan menolak di atas 100 MB, jadi file ini aman.
- Pengunjung perlu koneksi internet untuk memuat model-viewer (unpkg), three.js (cdnjs), dan font Google.
- Gunakan Git biasa atau upload lewat browser. Jika memakai Git, pastikan file `.glb` ikut ter-commit.

## Struktur

```
index.html
css/        tokens, base, layout, components, pages, fx, stage, backdrop-soda
js/         data, utils, vendor-loader, main, modules/ (termasuk soda-stage.js)
assets/img/ avatar, nebula, school
assets/3d/  bintang-1.glb + bintang-1-card.png (Zero), bintang-2.glb + bintang-2-card.png (Radler Lemon)
```
