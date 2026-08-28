# KLA BAST — Simulasi

Aplikasi percobaan untuk menu **Berita Acara Serah Terima (BAST)** dan **Pakta
Integritas** rekanan. Dipakai untuk ditinjau sebelum fiturnya dipasang ke
aplikasi KLA Ops yang sudah berjalan.

**Tidak ada data yang disimpan.** Semuanya di memori peramban — tidak ada
basis data, tidak ada `localStorage`, tidak ada permintaan ke mana pun. Halaman
ditutup, isinya hilang. Tombol **Reset simulasi** mengembalikan seperti semula.

Seluruh nama vendor, angka, dan nomor dokumen di dalamnya **fiktif**.

## Yang bisa dicoba

- Membuat berita acara dari nol, lalu mengganti kategorinya — tahap pengisian
  ikut berubah. Blok "Perubahan daya" hanya muncul untuk Kelistrikan / PLN;
  kolom volume dan kolom nomor seri saling bergantian menurut kategori.
- Memilih vendor dari Master Vendor. Vendor yang **NPWP/NIK, rekening, atau
  kontaknya kosong tidak bisa dipilih** — pagarnya sengaja ditunjukkan.
- Mencentang uji terima. Butir yang dijawab **Belum** menerbitkan tahap
  **Temuan** dengan sendirinya, dan berita acara tetap bisa terbit dengan
  status *diterima dengan catatan*.
- Menerbitkan dokumen: nomor diambil dari deret berjalan, lalu isinya terkunci.
- Mencetak: kop resmi berlogo, blok yang tidak relevan tidak ikut tercetak.
- Pakta Integritas: melekat pada vendor, berlaku 12 bulan sejak ditandatangani.

## Tanda tangan

Basah di atas meterai. **Tidak ada berkas yang diunggah** — aplikasi hanya
mencatat tanggalnya; lembar aslinya disimpan PIC.

## Menjalankan

Satu berkas `index.html`, tanpa pendamping dan tanpa proses build. Buka
langsung di peramban, atau taruh di hosting statis mana pun.

## Ini bukan aplikasi sungguhan

Aturan di dalamnya — kategori, blok yang menyala, kelengkapan vendor,
penomoran — ditulis ulang menyerupai modul yang sedang dibangun, supaya
simulasi ini tidak menjanjikan perilaku yang berbeda. Tetapi ia berdiri
sendiri: tidak menyentuh basis data, pengguna, maupun dokumen mana pun.
