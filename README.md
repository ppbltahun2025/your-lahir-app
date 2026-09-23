# Lahir App

Cek weton Jawa, zodiak Barat, shio Tionghoa, dan kohort generasi hanya dari satu tanggal lahir. Murni HTML, CSS, dan JavaScript — tidak ada dependency atau build step.

## Menjalankan secara lokal

Buka saja `index.html` langsung di browser. Tidak perlu server atau instalasi apa pun.

## Deploy ke GitHub Pages

1. Buat repository baru di GitHub, misalnya `lahir-app`.
2. Upload file `index.html` ini ke root repository (lewat web GitHub "Add file → Upload files", atau via git):
   ```bash
   git init
   git add index.html README.md
   git commit -m "Initial commit: Lahir App"
   git branch -M main
   git remote add origin https://github.com/USERNAME/lahir-app.git
   git push -u origin main
   ```
3. Di repository, buka **Settings → Pages**.
4. Pada **Source**, pilih branch `main` dan folder `/ (root)`, lalu **Save**.
5. Tunggu 1–2 menit, situs akan aktif di:
   ```
   https://USERNAME.github.io/lahir-app/
   ```

## Struktur file

```
lahir-app/
├── index.html   # seluruh aplikasi (HTML + CSS + JS dalam satu file)
└── README.md
```

## Catatan

- Rentang tanggal yang didukung: 1900–2026 (bisa diubah lewat atribut `min`/`max` pada input tanggal di `index.html`).
- Semua perhitungan (pasaran Jawa, zodiak, shio, generasi) dihitung langsung di browser, tidak ada request ke server luar selain memuat font dari Google Fonts.
