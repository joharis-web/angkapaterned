# 🔮 Mystic Number Engine – Realtime

- Auto fetch: Horoscope, Google, TikTok, Dream (via RapidAPI)
- Ekstrak keyword → cocokan ke dataset (erek)
- Kombinasi angka: **Erek + Shio + Zodiak + Jam** → 4 digit
- Tabel result, bisa **hapus baris** & **hapus semua** (localStorage)

## Deploy (Vercel)
1. Push project ini ke GitHub.
2. Vercel → New Project → pilih repo.
3. Tambah Environment Variable:
   - `RAPIDAPI_KEY` = API key RapidAPI kamu.
4. Deploy → buka URL Vercel → klik **Refresh & Fetch**.

> Penting: `vercel.json` sudah mengekspos `dataset.json`. Kalau angka tidak keluar, cek tab Network di browser:
> - `GET /dataset.json` harus status 200 dan berisi JSON (bukan HTML).
> - `GET /api/*` boleh gagal, tapi UI tetap menghasilkan angka fallback.
