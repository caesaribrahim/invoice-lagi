# Invoice Maker

Website statis (HTML/CSS/JS murni, tanpa build) untuk membuat, mencetak, dan menyimpan invoice.

## Fitur
- Form penerbit, klien, item, diskon (nominal / persen), PPN, biaya tambahan, info pembayaran, catatan
- Preview invoice live ukuran A4 (otomatis menyesuaikan layar)
- 3 template (Modern, Klasik, Minimal) + pilihan warna aksen
- Status invoice: Lunas (stempel) / Belum dibayar
- Terbilang otomatis untuk IDR, invoice bahasa Indonesia atau English
- Upload logo dan gambar tanda tangan
- Cetak langsung atau **Simpan sebagai PDF** (pilih "Save as PDF", matikan "Headers and footers")
- Simpan banyak invoice di browser (localStorage): cari, buka, duplikat, hapus
- Draf tersimpan otomatis saat mengetik, nomor invoice naik otomatis
- Export / Import JSON untuk backup atau pindah perangkat
- Shortcut: Ctrl+S simpan
- Tampilan mobile dengan tab Edit / Preview

## Jalankan lokal
Buka `index.html` di browser.

## Publish ke GitHub
`index.html` harus berada di root repo (bukan di dalam subfolder).

```bash
git init
git add .
git commit -m "Invoice maker"
git branch -M main
git remote add origin https://github.com/USERNAME/invoice-maker.git
git push -u origin main
```

## Deploy ke Vercel
1. Buka https://vercel.com/new dan import repo GitHub tadi.
2. Framework Preset: **Other**. Build Command dan Output Directory dibiarkan kosong.
3. Klik **Deploy**. Setiap `git push` akan otomatis deploy ulang.

Jika muncul 404: pastikan `index.html` ada di root repo dan Root Directory / Output Directory di pengaturan Vercel kosong.

## Catatan
Data tersimpan di browser masing-masing perangkat, bukan di server. Gunakan Export JSON untuk backup.
