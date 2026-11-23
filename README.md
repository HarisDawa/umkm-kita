# UMKMKita

Katalog produk UMKM per kecamatan. Belanja langsung dari pedagang & pengrajin lokal — chat WhatsApp, bayar di tempat, tanpa potongan.

Demo: https://umkm-kita.vercel.app

## Fitur

- Pencarian produk + filter kecamatan & kategori + urutan (laris/harga/rating)
- Kartu produk, modal detail, stepper jumlah, estimasi total live
- Form pesanan → pesan WhatsApp otomatis terisi
- Daftar UMKM pilihan, kategori, testimoni, FAQ, CTA pendaftaran

## Jalankan

Buka `index.html` di browser. Tanpa build, tanpa dependency.

## Kustomisasi

Semua data di `<script>` bagian bawah `index.html`:

- `WA_ADMIN` — nomor WhatsApp tujuan (format `62...`)
- `DATA` — daftar produk: `nama, toko, harga, satuan, kat, kec, emoji, grad, rating, terjual, halal, desc`

Ganti `emoji` + `grad` dengan `<img>` di `render()` bila sudah ada foto produk.

## Deploy

Static site, sudah dideploy ke Vercel. Push ke `main` lalu `vercel --prod`.
