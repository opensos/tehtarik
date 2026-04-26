# Teh Tarik — Jekyll Photo Journal

## Struktur Folder

```
teh-tarik-jekyll/
├── _config.yml          ← Tetapan laman (nama, url, dll)
├── _layouts/
│   └── default.html     ← Template HTML utama (header, font, dll)
├── _data/
│   └── photos.yml       ← Senarai gambar — EDIT DI SINI untuk tambah/buang gambar
├── img/                 ← Letak semua gambar anda di sini
├── index.html           ← Halaman utama (pakai Liquid loop dari photos.yml)
├── Gemfile
└── README.md
```

## Cara Guna

### 1. Install Jekyll
```bash
gem install bundler jekyll
bundle install
```

### 2. Jalankan secara lokal
```bash
bundle exec jekyll serve
```
Buka `http://localhost:4000`

### 3. Tambah Gambar Baru
- Salin gambar ke folder `img/`
- Tambah entry baru dalam `_data/photos.yml`:

```yaml
- src: /img/nama-gambar.jpg
  alt: Nama alternatif
  caption: Teks kapsyen (optional)
```

### 4. Deploy ke GitHub Pages
1. Push folder ini ke repo GitHub
2. Pergi ke Settings → Pages → pilih branch `main`
3. GitHub akan build Jekyll secara automatik

## Nota
- Gambar luar (URL penuh) masih berfungsi — letak URL terus dalam `src`
- Untuk tukar font atau warna, edit `_layouts/default.html`
- Untuk tukar title laman, edit `_config.yml`
