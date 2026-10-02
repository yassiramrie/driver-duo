# Driver Duo

Landing page profil dua pembalap bergaya F1: **Yassir Army Tigreal** (#44) dan **Alveoniro Moskop Epic** (#69). Satu halaman berisi hero, biografi, statistik, dan karier; klik avatar di hero untuk berganti pembalap.

Dibangun dengan Next.js 16 (App Router), TypeScript, dan Tailwind CSS 4.

## Menjalankan secara lokal

Butuh Node.js 20.9 atau lebih baru.

```bash
npm ci
npm run dev      # mode development di http://localhost:3000
```

Untuk mode produksi:

```bash
npm run build
npm start
```

## Struktur

| Path | Isi |
| --- | --- |
| `app/page.tsx` | Halaman utama; atur `defaultDriver` dan `autoRotate` di sini |
| `app/api/health/route.ts` | Endpoint health check, `GET /api/health` |
| `components/` | Hero, header, peta sirkuit, dan section Biografi/Statistik/Karier |
| `lib/drivers.ts` | Semua data pembalap (data dummy, ganti di sini) |
| `public/drivers/` | Foto cutout pembalap |

## Tugas Docker

Repo ini sengaja belum punya `Dockerfile`. Instruksi lengkapnya ada di [TASKS.md](TASKS.md).
