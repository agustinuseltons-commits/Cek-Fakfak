# Cek Fakfak — kerangka situs

Situs statis: tanpa database, tanpa login, tanpa biaya hosting. Semua file bisa diedit dengan editor teks apa pun (Notepad, VS Code).

## Isi paket

```
index.html       beranda + edisi terbaru
seri.html        arsip semua edisi
data.html        daftar dataset yang bisa diunduh
metode.html      cara membaca data dan batasnya (ditulis sekali, dirujuk selamanya)
tentang.html     siapa Anda + disclaimer
style.css        tampilan; satu font, tanpa framework
edisi/001.html   TEMPLATE edisi — salin untuk edisi berikutnya
data/            taruh file CSV di sini (+ CHANGELOG.md)
img/             buat folder ini untuk grafik PNG/SVG
```

Yang masih harus Anda isi: semua teks dalam `[kurung siku]`, alamat email di footer, dan tautan sumber.

## Menerbitkan edisi baru

1. Salin `edisi/001.html` → `edisi/002.html`. Isi.
2. Simpan grafik sebagai `img/002.png` (atau SVG). Simpan data mentahnya sebagai `data/<nama>.csv`.
3. Tambahkan satu baris `<li>` di `seri.html` (paling atas) dan ganti baris "Edisi terbaru" di `index.html`.
4. Tambahkan baris di tabel `data.html` kalau ada dataset baru.
5. Unggah (lihat di bawah).

## Memasang gratis di GitHub Pages

1. Buat akun GitHub. Buat repositori baru, nama bebas (misalnya `fakfak-dalam-data`), **Public**.
2. Unggah semua file dalam folder ini ke repositori (tombol *Add file → Upload files*, atau lewat Git).
3. Buka *Settings → Pages*. Pada *Source* pilih **Deploy from a branch**, branch `main`, folder `/ (root)`. Simpan.
4. Dalam 1–2 menit situs aktif di `https://<username>.github.io/fakfak-dalam-data/`.
5. Untuk domain sendiri (misalnya `eltonsesa.id`): beli domain di registrar Indonesia (PANDI-accredited: Niagahoster, Rumahweb, dll.), lalu di *Settings → Pages → Custom domain* masukkan nama domain, dan di registrar tambahkan record DNS sesuai petunjuk GitHub (A record ke IP GitHub Pages, atau CNAME ke `<username>.github.io`). Centang *Enforce HTTPS* setelah aktif.

Alternatif dengan cara yang sama: Cloudflare Pages, Netlify (keduanya gratis untuk situs statis). Kalau ingin langganan email pembaca tanpa repot, Substack bisa dipakai sebagai kanal pengiriman dan situs ini sebagai arsip+data.

## Tiga aturan yang sebaiknya tidak dilanggar

- Hanya data publik dengan tautan. Tidak ada "menurut sumber di Pemkab".
- Deskriptif, bukan evaluatif. Pembaca yang menyimpulkan.
- Tidak menyentuh urusan perhubungan.

## Sebelum edisi #1 terbit

Tanyakan ke BKPSDM Kabupaten Fakfak apakah ada surat edaran atau peraturan bupati tentang pernyataan publik / media sosial ASN. Lebih murah bertanya dulu daripada menjelaskan kemudian.
