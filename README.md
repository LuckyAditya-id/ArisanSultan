# Arisan Sultan – kocokan online (2 pemenang per putaran)

Netlify Functions + Netlify Blobs. Tanpa database luar, tanpa akun.

## Deploy
1. Buat repo GitHub baru, unggah isi folder ini (package.json, netlify.toml, folder public/ dan netlify/).
2. Netlify → Add new site → Import from Git → pilih repo (build otomatis terbaca dari netlify.toml).
3. Bagikan tautan situs ke grup.

## Mengubah data
- Daftar peserta & yang sudah menang: `netlify/functions/core.mjs` (IDS, DEFAULT_NAMES, BASE) dan `public/index.html` (PEOPLE, BASE_IDS).
- Jumlah pemenang per putaran: PER_ROUND (core.mjs).
- Mulai ulang dari awal: Netlify → Blobs → hapus store `arisan-sultan`.
