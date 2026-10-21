# Ciflow Florist

Prototype Next.js App Router dengan UI pastel pink/peach bergaya bold-outline dashboard. Terinspirasi dari gambar referensi yang diberikan pengguna, bukan salinan kode/aset situs lain.

## Menjalankan

```bash
npm install
npm run dev
```

Buka http://localhost:3000

## Fitur demo

- Dashboard statistik dan pesanan
- Katalog produk florist
- Keranjang dan checkout
- Simulasi pembayaran (tidak ada QRIS aktif)
- Pesanan dan tracking status simulasi
- Manajemen produk dan laporan ilustratif
- Responsif desktop/mobile

## Penting

Semua data saat ini berada di React state dan kembali ke data awal setelah refresh. **Belum** terhubung Supabase, Midtrans, maupun API pengiriman. Jangan gunakan simulasi pembayaran untuk transaksi sungguhan.

## Deploy

Upload repo ke GitHub, lalu Import Project di Vercel (Framework: Next.js). Tidak membutuhkan environment variables untuk versi demo.

## Website pelanggan (baru)
- `/toko` adalah storefront khusus pelanggan, terpisah dari dashboard admin `/`.
- Alur: beranda → katalog → keranjang → checkout → pembayaran demo → tracking demo.
- Keranjang dan pesanan demo disimpan di localStorage browser. Dashboard admin dapat membaca pesanan demo dari browser yang sama setelah halaman dimuat ulang. Ini **bukan** sinkronisasi antar perangkat dan **bukan** database produksi.
- Tarif pengiriman dan QRIS hanyalah ilustrasi. Belum ada integrasi Midtrans, Supabase, atau API kurir sungguhan.
