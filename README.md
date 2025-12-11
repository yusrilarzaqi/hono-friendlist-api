# Friendlist API Hono + Bun

Friendlist API adalah proyek backend ringan yang dibangun menggunakan Hono
(framework web super cepat untuk TypeScript) dan Bun sebagai runtime modern
yang sangat cepat. API ini dirancang untuk mengelola daftar pertemanan dengan performa
tinggi serta struktur kode yang sederhana dan mudah dikembangkan.

## Fitur Utama

- 🚀 Cepat, ringan, dan minimalis
- 🧩 CRUD lengkap untuk data friendlist
- 📦 Routing modular menggunakan Hono
- ⚡ Bun runtime untuk eksekusi super cepat
- 🔒 Validasi input opsional (Zod atau custom)
- 📚 Kode bersih & mudah dikembangkan

## Toknologi

- Bun runtime JavaScript modern & kencang
- Hono web framework ringan & performa tinggi
- TypeScript untuk type safety
- Database Postgresql
- ORM Prisma

## Struktur Project

### Service

- `src/app/auth.service.ts` : Service untuk mengelola data autentikasi
- `src/app/user.service.ts` : Service untuk mengelola data user
- `src/app/friend.service.ts` : Service untuk mengelola data teman

### Controller

- `src/controllers/auth.controller.ts` : Controller untuk mengelola data autentikasi
- `src/controllers/user.controller.ts` : Controller untuk mengelola data user
- `src/controllers/friend.controller.ts` : Controller untuk mengelola data teman

### Middleware

- `src/middleware/auth.middleware.ts` : Middleware untuk mengelola data autentikasi
- `src/middleware/error.middleware.ts` : Middleware untuk menangani kesalahan
- `src/middleware/validate.middleware.ts` : Middleware untuk memvalidasi input
- `src/middleware/limit.middleware.ts` : Middleware untuk membatasi jumlah request

## Endpoint

### Auth endpoint

- `POST /auth/login` : Login
- `POST /auth/register` : Register
- `POST /auth/logout` : Logout
- `POST /auth/refresh` : Refresh token

### User endpoint

- `GET /users` : Mendapatkan daftar user
- `POST /users` : Menambahkan user baru
- `PUT /users/:id` : Memperbarui user
- `DELETE /users/:id` : Menghapus user

### Friends endpoint

- `GET /friends` : Mendapatkan daftar teman
- `POST /friends` : Menambahkan teman baru
- `PUT /friends/:id` : Memperbarui teman
- `DELETE /friends/:id` : Menghapus teman

## Tujuan project

Project ini dibuat sebagai contoh implementasi API modern menggunakan Hono + Bun, cocok untuk:

- belajar backend cepat dan minimalis
- eksperimen dengan Bun runtime
- membuat layanan microservice ringan
- latihan membuat REST API

## Instalasi

1. Clone repository

```bash
git clone https://github.com/yusrilarzaqi/hono-friendlist-api

cd hono-friendlist-api
```

2. Install dependencies

```
bun install
```

3. Run development server

```
bun run --hot src/index.ts
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Kontribusi

Jika Anda tertarik untuk berkontribusi, silakan fork repository ini dan buat pull request. Terima kasih!

## License

MIT License, Copyright (c) 2023 Yusril Arzaqi
