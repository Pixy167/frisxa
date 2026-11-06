# A Letter for Osi (Vercel)

Situs statis, tanpa build. Isinya: `index.html` + folder `assets/`.

## Deploy
**Vercel CLI**
```
npm i -g vercel
cd letter-for-osi
vercel --prod
```
**Lewat GitHub**: upload folder ini ke repo, lalu vercel.com/new, pilih repo, Framework Preset: *Other*, kosongkan Build Command dan Output Directory, Deploy.

## Tes lokal
Buka lewat server, jangan klik dua kali (fetch tidak jalan di file://):
```
npx serve .          # atau: python3 -m http.server 3000
```

## Ganti isi
- Lagu: timpa `assets/song.mp3` (judul di kartu musik ada di `index.html`, cari "Love Nwantiti")
- Foto: `assets/img/01.jpg` sampai `10.jpg`
- Beruang: `assets/bear.bin`, buket: `assets/bouquet.fbx` + `assets/leaf-*.png`

## Catatan
- three.js dimuat dari CDN (jsDelivr), jadi perlu internet.
- Suara "I love you" memakai suara bawaan browser/HP, jadi bunyinya bisa beda di tiap perangkat.
- Halaman diberi noindex supaya tidak muncul di Google.
