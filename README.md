# Invoice Maker

Website statis (HTML/CSS/JS murni, tanpa build) untuk membuat, mencetak, dan menyimpan invoice.

## Fitur
- Form penerbit, penerima, item, pajak, diskon, info pembayaran, catatan
- Preview invoice live (ukuran A4)
- Cetak langsung atau **Simpan sebagai PDF** (tombol Cetak, pilih "Save as PDF")
- Simpan banyak invoice di browser (localStorage), buka & hapus kembali
- Export / Import JSON untuk backup atau pindah perangkat
- Upload logo perusahaan

## Jalankan lokal
Buka `index.html` di browser.

## Publish ke GitHub
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
3. Klik **Deploy**. Selesai, setiap `git push` akan otomatis deploy ulang.

## Catatan
Data tersimpan di browser masing-masing perangkat, bukan di server. Gunakan Export JSON untuk backup.
