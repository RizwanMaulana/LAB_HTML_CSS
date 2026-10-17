# Jawaban Praktikum: Rizwan Maulana (10224083)

## Bagian 1: Pemanasan

1. Pada aturan nav a.active:hover { color: red; }:
   - Selector: nav a.active:hover
   - Deklarasi: { color: red; }
   - Property: color
   - Value: red
   - Pseudo-class: :hover

2. Block: p, li, h2 | Inline: span, a, strong

3. Paragraf A dan B jadi hijau (karena di dalam div class="box"). C dan D tidak.

4. Warnanya MERAH (red). Karena #title (ID selector) punya spesifisitas tertinggi (100) dibanding .heading (10) dan h1 (1).

5. Tag strong ditutup setelah /p, seharusnya ditutup sebelum /p. Benar: <p>Hello <strong>world</strong></p>

## Bagian 3: Prediksi Selector Golf

P1:
(a) Weekly hack nights = HIJAU (section p lebih spesifik dari p)
(b) Bring your own laptop = HIJAU (section p lebih spesifik dari .note)
(c) 2026 Student Affairs = BIRU (hanya p yang apply, tidak di dalam section)

P2. Urutan spesifisitas tertinggi ke terendah:
1. #tech p (ada ID)
2. .club p (ada class)
3. main section p (3 element)
4. p (1 element)

## Bagian 4: Box Model

Q1. Lebar terlihat = 300 + 16+16 + 1+1 = 334px
Q2. Dengan border-box, lebar total tetap 300px (padding dan border sudah termasuk)

## Bagian 5: Tabel Debug

| # | Baris | Bug | Perbaikan | Cara menemukan |
|---|-------|-----|-----------|----------------|
| 1 | colour: #333 | Typo | color: #333 | DevTools property dicoret |
| 2 | background: #dbe7f3 | Kurang ; | tambah ; | Validator error |
| 3 | .Card | Case sensitive | .card | Class di HTML lowercase |
| 4 | 18 px | Spasi | 18px | DevTools tidak apply |
| 5 | centre | Typo | center | DevTools property dicoret |
| 6 | h1.../h2 | Tag tidak match | h1.../h1 | Validator error |
| 7 | img tanpa alt | Aksesibilitas | tambah alt | Validator warning |
| 8 | #news-list vs newsList | ID tidak match | samakan | Styling tidak apply |
| 9 | nav tanpa ul | Tidak semantik | tambah ul/li | Best practice |

## Bagian 6: Code Review

| # | Masalah | Mengapa penting | Perbaikan |
|---|---------|-----------------|-----------|
| 1 | Tidak ada DOCTYPE | Quirks mode | Tambah DOCTYPE |
| 2 | Pakai div bukan header | Tidak semantik | Ganti header |
| 3 | Pakai b bukan h1 | Tidak semantik | Ganti h1 |
| 4 | Pakai div bukan nav | Tidak semantik | Ganti nav |
| 5 | Ada !important | Bad practice | Hapus !important |
| 6 | Inline style | Sulit maintain | Pindah ke CSS |
| 7 | Float untuk layout | Outdated | Pakai flexbox |
| 8 | Pakai div bukan main | Tidak semantik | Ganti main |

Refleksi:
1. Inline style dan !important paling sulit disadari karena halaman tetap terlihat baik.
2. Masalah semantik penting untuk aksesibilitas, SEO, dan maintenance.
3. Kebiasaan: selalu validasi dengan W3C Validator sebelum submit.

## Bagian 7: Exit Ticket

1. Aturan CSS = selector + declaration block (property: value). Contoh: h1 { color: red; }
2. Spesifisitas selector masih agak membingungkan.
3. Membuat struktur HTML semantik (header, nav, main, footer) tanpa perlu lihat dokumentasi.
