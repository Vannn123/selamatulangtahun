# 🎂 Birthday Website

Website ulang tahun interaktif dengan tema ungu dan kucing lucu!

## ✨ Fitur
- 🕯️ Animasi kue dengan lilin yang bisa ditiup (klik atau mic)
- 💌 Kartu ucapan interaktif
- 📸 5 kotak kenangan (bisa diisi foto sendiri)
- 🌱 Timeline perkembangan (bayi → anak → remaja)
- 🎵 Musik otomatis saat dibuka
- 🔒 Tombol "cie 21 tahun" yang kabur-kaburan
- 🐱 Kucing di mana-mana!

## 🛠️ Cara Kustomisasi

### Ganti Musik
1. Taruh file musik kamu di folder ini dengan nama `music.mp3`
2. Atau ganti baris ini di `index.html`:
   ```html
   <source src="music.mp3" type="audio/mpeg">
   ```
   Ganti `music.mp3` dengan nama file musikmu.

### Ganti Foto Kenangan
Di bagian `<!-- Memory 1 -->` hingga `<!-- Memory 5 -->`, ganti:
```html
<div class="memory-photo-placeholder">
  <span class="ph-icon">📷</span>
  <span>Foto Kenangan 1</span>
</div>
```
Dengan:
```html
<img src="foto1.jpg" alt="Kenangan 1" style="width:100%;height:200px;object-fit:cover;">
```

### Ganti Foto Perkembangan
Di bagian `<!-- Baby -->`, `<!-- Child -->`, `<!-- Teen -->`, ganti:
```html
<div class="growth-placeholder">...</div>
```
Dengan:
```html
<img src="bayi.jpg" alt="Bayi">
```

### Ganti Teks Ucapan
Cari section `<!-- ===== SECTION 2: CARD ===== -->` dan edit teks di dalam tag `<p>`.

## 🚀 Cara Upload ke GitHub Pages

### Langkah 1: Buat akun GitHub
Daftar di [github.com](https://github.com) jika belum punya.

### Langkah 2: Buat repository baru
1. Klik tombol **+** → **New repository**
2. Nama repo: `birthday-website` (atau nama lain)
3. Pilih **Public**
4. Klik **Create repository**

### Langkah 3: Upload file
**Cara mudah (drag & drop):**
1. Di halaman repo, klik **uploading an existing file**
2. Drag & drop file `index.html` (dan `music.mp3` jika ada, dan foto-foto)
3. Scroll ke bawah, klik **Commit changes**

**Atau via Git:**
```bash
git init
git add .
git commit -m "Birthday website"
git branch -M main
git remote add origin https://github.com/USERNAME/birthday-website.git
git push -u origin main
```

### Langkah 4: Aktifkan GitHub Pages
1. Di repo, klik **Settings**
2. Scroll ke **Pages** (di sidebar kiri)
3. Pada **Source**, pilih **Deploy from a branch**
4. Pilih branch **main**, folder **/ (root)**
5. Klik **Save**

### Langkah 5: Website online! 🎉
Tunggu 1-2 menit, lalu aksesnya di:
```
https://USERNAME.github.io/birthday-website/
```
Ganti `USERNAME` dengan username GitHub kamu.

## 📁 Struktur File
```
birthday-website/
├── index.html      ← File utama website
├── music.mp3       ← File musik (taruh sendiri)
├── foto1.jpg       ← Foto kenangan 1 (opsional)
├── foto2.jpg       ← Foto kenangan 2 (opsional)
├── foto3.jpg       ← Foto kenangan 3 (opsional)
├── foto4.jpg       ← Foto kenangan 4 (opsional)
├── foto5.jpg       ← Foto kenangan 5 (opsional)
├── bayi.jpg        ← Foto bayi (opsional)
├── anak.jpg        ← Foto anak-anak (opsional)
├── remaja.jpg      ← Foto remaja (opsional)
└── README.md       ← File ini
```

---
Made with 💜 and lots of 🐱
