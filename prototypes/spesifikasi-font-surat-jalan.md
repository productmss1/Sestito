# 📄 Spesifikasi Tipografi & Font Size Surat Jalan (A5 Landscape)

Dokumen ini memuat spesifikasi teknis lengkap mengenai **Font Family**, **Font Size (px)**, **Font Weight (Ketebalan)**, **Line Height**, **Perataan Teks (*Alignment*)**, serta **Warna Teks** yang diekstrak langsung dari desain purwarupa [`prototypes/surat-jalan.html`](file:///Users/admin/Documents/Product%20Space/Antigravity/Product%20Space/prototypes/surat-jalan.html).

---

## 🎨 1. Spesifikasi Umum Dokumen (Global Setup)

* **Font Family:** `'Helvetica Neue', Helvetica, Arial, sans-serif`
* **Base Font Size:** `11px`
* **Warna Teks Utama:** `#000000` (Hitam pekat)
* **Ukuran Kertas Cetak:** A5 Landscape (**210mm × 148mm**)
* **Padding Lembar Cetak (*Sheet*):** `1.5mm 8mm 4mm 8mm` (Atas: `1.5mm`, Kanan: `8mm`, Bawah: `4mm`, Kiri: `8mm`)
* **Border Garis Tabel:** `1px solid #000000` (Tabel terstruktur dengan border penuh)
* **Padding Sel Tabel Standar:** `6px 8px` (Header & Alamat) / `4px 6px` (Isi Tabel & Header Meta)

---

## 📑 2. Bagian Indikator Halaman (Page Number)

Diposisikan di pojok kanan atas lembar cetak sebelum tabel header.

| Elemen | Font Size (px) | Font Weight | Line Height / Alignment | Warna Hex / Deskripsi |
| :--- | :---: | :---: | :---: | :--- |
| **Indikator Halaman** (`1 dari 1`) | **`10px`** | Regular (400) | Right / `margin-bottom: 2px` | `#000000` |

---

## 🏢 3. Bagian Header Dokumen (`.header-table`)

Tabel header terbagi menjadi 3 kolom: Area Logo (15%), Area Judul Dokumen & Identitas Perusahaan (60%), dan Area Metadata Dokumen (25%).

| Bagian / Elemen | Font Size (px) | Font Weight | Perataan (*Align*) | Deskripsi / Warna |
| :--- | :---: | :---: | :---: | :--- |
| **Logo Cell** (`[LOGO]`) | **`14px`** | Bold (700) | Center | `#000000` (Lebar kolom 15%) |
| **Judul Utama (`h1`)**<br>`SURAT JALAN PENGIRIMAN` | **`14px`** | Bold (700) | Center | `#000000`, `letter-spacing: 0.5px`, `margin-bottom: 2px` |
| **Nama Perusahaan / Toko (`h2`)**<br>`PT. POS INDONESIA` | **`11px`** | Bold (700) | Center | `#000000`, `margin-bottom: 2px` |
| **Alamat & Telepon Toko (`p`)**<br>`Jl. Banda No. 30... \| Telp: ...` | **`9px`** | Regular (400) | Center | `#333333` |
| **Label Metadata**<br>`No. Surat Jalan:`, `No. Transaksi:`, `Tanggal:` | **`10px`** | Regular (400) | Left | `#000000`, `line-height: 1.15` |
| **Nilai Metadata (`.value`)**<br>`PNG-01-20260101-00123`, `TRN/...`, `01 Januari 2026` | **`10px`** | Bold (700) | Left | `#000000`, `margin-bottom: 4px` |

---

## 📍 4. Bagian Informasi Alamat (`.address-table`)

Tabel alamat terbagi simetris 2 kolom (masing-masing 50%): Kolom Pengirim dan Kolom Penerima dengan tinggi tetap `height: 65px`.

| Elemen | Font Size (px) | Font Weight | Line Height | Deskripsi / Warna |
| :--- | :---: | :---: | :---: | :--- |
| **Header Kolom** (`PENGIRIM`, `PENERIMA`) | **`10px`** | Bold (700) | Normal | `#000000`, Uppercase, Left-aligned |
| **Label Field** (`Nama:`, `Alamat:`, `HP:`, `Telp:`) | **`10px`** | Bold (700) | `1.4` | `#000000`, `display: inline-block`, `width: 45px` |
| **Nilai Field** (Nama Toko/Penerima, Alamat Lengkap, No. Kontak) | **`10px`** | Regular (400) | `1.4` | `#000000` |

---

## 📦 5. Bagian Tabel Produk (`.product-table`)

Tabel daftar barang yang dikirim dengan kapasitas maksimal 8 baris produk per halaman A5 Landscape.

| Kolom | Lebar (*Width*) | Font Size (px) | Font Weight | Perataan (*Align*) | Padding Sel |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Header Tabel** (`NO`, `NAMA PRODUK`, `JUMLAH`, `SATUAN`) | Sesuai Kolom | **`10px`** | Bold (700) | Center | `6px 8px` |
| **Kolom No** (1 s/d 8) | `5%` | **`10px`** | Regular (400) | Center | `4px 6px` |
| **Kolom Nama Produk** (`Semen Tiga Roda 40 Kg`, dll.) | `70%` | **`10px`** | Regular (400) | Left | `4px 6px` |
| **Kolom Jumlah** (`1`, `10`, dll.) | `12%` | **`10px`** | Regular (400) | Center | `4px 6px` |
| **Kolom Satuan** (`sak`, `pcs`, `boks`, dll.) | `13%` | **`10px`** | Regular (400) | Center | `4px 6px` |

---

## ✍️ 6. Bagian Footer & Tanda Tangan (`.footer-table`)

Tabel footer terbagi 4 kolom sama rata (masing-masing 25%) dengan tinggi sel tetap `height: 75px` yang memuat Catatan dan 3 Kolom Tanda Tangan fisik.

| Kolom / Komponen | Font Size (px) | Font Weight | Perataan (*Align*) | Deskripsi / Warna |
| :--- | :---: | :---: | :---: | :--- |
| **Header Footer** (`CATATAN`, `KEPALA GUDANG`, `PENGIRIMAN`, `PENERIMA`) | **`10px`** | Bold (700) | Center | `#000000`, Uppercase |
| **Isi Catatan (`.catatan-content`)** | **`10px`** | Regular (400) | Left | `#333333` |
| **Garis / Titik Tanda Tangan (`.signature-line`)**<br>`(....................)` | **`10px`** | Regular (400) | Center | `#000000`, `margin-top: auto` |
| **Keterangan Bawah TTD (`.signature-sub`)**<br>`Nama & Tanda Tangan` | **`9px`** | Regular (400) | Center | `#000000`, `margin-top: 2px` |

---

## 🖥️ 7. Bagian Kontrol Antarmuka Web / No-Print (`.no-print-container`)

Elemen bar navigasi preview pada layar web (tidak ikut tercetak saat diprint).

| Elemen | Font Size (px) | Font Weight | Warna Hex / Deskripsi |
| :--- | :---: | :---: | :--- |
| **Judul Bar Preview** (`Desain Surat Jalan A5 Landscape`) | **`13px`** | Bold (700) | `#1e3a8a` |
| **Subjudul Bar Preview** (`Tampilan presisi...`) | **`11px`** | Regular (400) | `#1d4ed8` |
| **Tombol "← Kembali ke Hub"** | **`12px`** | Bold (700) | `#f97316` (Bg: `#1e293b`) |
| **Tombol "Cetak Surat Jalan"** | **`12px`** | Bold (700) | `#ffffff` (Bg: `#2563eb`) |
| **Tombol "Export PNG"** | **`12px`** | Bold (700) | `#ffffff` (Bg: `#10b981`) |

---

## 📌 Ringkasan Hierarki Ukuran Font (Summary Quick Reference)

```
┌──────────────┬─────────────────────────────────────────────────────────────────────────────┐
│ Ukuran (px)  │ Penerapan Elemen pada Desain Surat Jalan                                    │
├──────────────┼─────────────────────────────────────────────────────────────────────────────┤
│ 14px         │ • [LOGO] placeholder (Bold)                                                 │
│              │ • Judul Dokumen Utama "SURAT JALAN PENGIRIMAN" (h1, Bold)                   │
├──────────────┼─────────────────────────────────────────────────────────────────────────────┤
│ 13px         │ • Judul Bar Navigasi/Preview Web (h3, Bold)                                 │
├──────────────┼─────────────────────────────────────────────────────────────────────────────┤
│ 12px         │ • Tombol Aksi Web (Cetak Surat Jalan, Export PNG, Kembali ke Hub)           │
├──────────────┼─────────────────────────────────────────────────────────────────────────────┤
│ 11px         │ • Nama Toko/Perusahaan Header (h2, Bold)                                    │
│              │ • Sub-deskripsi Bar Preview Web                                             │
├──────────────┼─────────────────────────────────────────────────────────────────────────────┤
│ 10px         │ • Indikator Halaman (Page Number: "1 dari 1")                               │
│              │ • Label & Nilai Metadata Dokumen (No. SJ, No. TRN, Tanggal)                 │
│              │ • Header Kolom PENGIRIM & PENERIMA                                          │
│              │ • Label & Nilai Alamat Pengirim & Penerima                                  │
│              │ • Header Tabel Produk (NO, NAMA PRODUK, JUMLAH, SATUAN)                     │
│              │ • Seluruh Isi Baris Tabel Produk (No, Nama Produk, Jumlah, Satuan)          │
│              │ • Header Footer (CATATAN, KEPALA GUDANG, PENGIRIMAN, PENERIMA)              │
│              │ • Isi Teks Catatan Pengiriman                                               │
│              │ • Titik-titik Kolom TTD "(....................)"                            │
├──────────────┼─────────────────────────────────────────────────────────────────────────────┤
│ 9px          │ • Alamat & Telp Toko/Perusahaan di Header Tengah                            │
│              │ • Keterangan Bawah TTD "Nama & Tanda Tangan"                                │
└──────────────┴─────────────────────────────────────────────────────────────────────────────┘
```
