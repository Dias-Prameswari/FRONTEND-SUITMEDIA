# FRONTEND-SUITMEDIA

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Proyek Frontend untuk Suitmedia menggunakan **Next.js** dan **TailwindCSS**.

## Deskripsi Proyek

- Menggunakan Next.js App Router (React Server Components + Client Components).
- Menggunakan TailwindCSS untuk styling.
- Memiliki fitur header dengan navigasi yang responsif dan animasi scroll.
- Halaman utama menampilkan banner dan daftar postingan dengan pagination, sorting, dan filter.
- Data postingan diambil dari API backend Suitmedia.
- Mendukung dynamic routing dan state URL (query params).

## Struktur Folder Penting

- src/app - Folder utama berisi halaman (pages) dan routing.
- src/components - Komponen React yang digunakan pada halaman.
- src/components/ui - Komponen UI seperti Select dropdown.
- public - Folder berisi aset statis seperti gambar logo.

## Cara Menjalankan
1. Clone repository ini
2. Masuk ke folder proyek : cd FRONTEND-SUITMEDIA
3. Install dependencies: npm install
4. Jalankan mode development: npm run dev
5. Jalankan build production: npm run build

## Penjelasan Komponen Utama 
1. Header : Menampilkan navigasi utama dengan animasi saat scroll dan indikator halaman aktif
2. Banner : Menampilkan gambar banner dengan efek parallax dan overlay warna
3. ListPost : Menampilkan daftar postingan dari API dengan pagination, filter ukuran halamn, dan sorting
4. Pagination : Komponen pagination untuk navigasi halaman postingan
5. PostCard : Menampilkan kartu postingan dengan gambar, tanggal dan judul

## Catatan
Pastikan saat development dan build tidak ada error terkait penggunaan useSearchParams dan Suspense. Komponen yang memerlukan client-side rendering menggunakan "use client" directive. Untuk build di vercel, pastikan environment dan dependencies sudah sesuai

This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
