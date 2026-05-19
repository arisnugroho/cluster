# The Palace · Dashboard IPL

Dashboard transparansi keuangan warga berbasis web.  
Siap deploy ke Vercel sebagai static site.

---

## 🗂 Struktur File

```
/
├── index.html      ← Dashboard utama (satu file, semua halaman)
├── vercel.json     ← Konfigurasi Vercel
└── README.md       ← Panduan ini
```

---

## 🚀 Cara Deploy ke Vercel

### Opsi A — Via GitHub (Direkomendasikan)

1. Buat repository baru di [github.com](https://github.com)
2. Upload ketiga file ini (`index.html`, `vercel.json`, `README.md`)
3. Buka [vercel.com](https://vercel.com) → **Add New Project**
4. Import repository GitHub tadi
5. Biarkan semua setting default → klik **Deploy**
6. ✅ Dashboard langsung live di `https://nama-project.vercel.app`

### Opsi B — Via Vercel CLI

```bash
# Install Vercel CLI
npm i -g vercel

# Masuk ke folder project
cd folder-dashboard

# Deploy
vercel

# Ikuti prompt, pilih defaults semua
```

### Opsi C — Drag & Drop (Paling Mudah)

1. Buka [vercel.com/new](https://vercel.com/new)
2. Drag & drop **folder** berisi ketiga file
3. Klik Deploy → selesai

---

## 🔐 Kredensial Demo

| Role       | Username | Password   |
|------------|----------|------------|
| Warga      | warga    | warga123   |
| Super Admin | admin   | admin123   |

> **Catatan:** Kredensial ini hardcoded untuk demo.  
> Setelah integrasi Google Sheets / backend, ganti dengan autentikasi sesungguhnya.

---

## 🔧 Kustomisasi

### Ganti nama kompleks
Cari `The Palace` di `index.html` → ganti dengan nama kompleks Anda.

### Tambah/ubah data warga
Edit array `WARGA_DATA` di bagian `<script>` di dalam `index.html`.

### Ubah data transaksi
Edit array `TR_DATA` di bagian `<script>`.

---

## 📋 Fitur

- ✅ Login dua role: Warga & Super Admin
- ✅ Dashboard dengan KPI, donut chart, bar chart, line chart
- ✅ Halaman IPL Bulanan dengan filter status
- ✅ Halaman Transaksi dengan filter tipe
- ✅ Laporan keuangan dengan area chart tren saldo
- ✅ Data Warga (Admin only)
- ✅ Dark mode / Light mode
- ✅ Toggle sembunyikan jumlah (privacy mode)
- ✅ Session login (tetap login setelah refresh)
- ✅ Responsive layout

---

## 🗺 Roadmap (Backend Integration)

- [ ] Google Sheets API — data real-time
- [ ] Google Apps Script — autentikasi aman
- [ ] Export PDF laporan per bulan
- [ ] Notifikasi warga belum bayar
- [ ] Upload bukti pembayaran

---

*Dibuat untuk transparansi keuangan warga · The Palace Cluster*
