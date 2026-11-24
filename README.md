# LpDeFiPie

Aplikasi web berbasis Next.js (App Router) dengan Tailwind CSS, yang telah dikonfigurasi agar siap dijalankan di dalam kontainer Docker menggunakan mode `standalone`.

## Teknologi Utama
- **Framework:** Next.js (TypeScript)
- **Styling:** Tailwind CSS
- **Containerization:** Docker & Docker Compose (Multi-stage Alpine build)

## Cara Menjalankan

### Opsi 1: Menggunakan Docker (Direkomendasikan)
Pastikan Docker Engine, Docker Desktop, atau Kiri sudah berjalan di perangkatmu.

1. Build dan jalankan kontainer di latar belakang:
   `docker compose up -d --build`
2. Buka browser dan akses `http://localhost:3000`.
3. Untuk menghentikan kontainer:
   `docker compose down`

### Opsi 2: Menjalankan Secara Lokal (Tanpa Docker)
1. Install dependensi:
   `npm install`
2. Jalankan server development:
   `npm run dev`
3. Buka `http://localhost:3000` di browser.

## Struktur Proyek
- `src/app/` — Halaman utama, layout, dan styling global.
- `src/template/` — Komponen bagian halaman (*Header*, *Footer*, *Vision*, *Pipeline*, dll.).
- `public/` — Aset statis dan gambar.
- `Dockerfile` & `docker-compose.yml` — Konfigurasi build dan orkestrasi kontainer produksi.