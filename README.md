
<center><img src ="icon/icon.png" width="200" height="200"></center>

---

# **Coffie Shop**  
*Aplikasi Pemesanan Kopi Online Modern*

## **Deskripsi**  
**Coffie Shop** adalah platform e-commerce berbasis web yang dirancang khusus untuk kedai kopi, memungkinkan pelanggan memesan minuman secara online dengan mudah. Aplikasi ini mencakup manajemen menu, pemesanan, pembayaran digital, dan analitik penjualan untuk pemilik bisnis.  

Target Pengguna:  
- **Pelanggan**: Memesan kopi, melihat riwayat transaksi, dan membayar secara digital.  
- **Admin/Pemilik**: Mengelola menu, stok, pesanan, dan laporan penjualan.  

---

## **Fitur Utama**  

### **1. Untuk Pelanggan**  
- **Antarmuka Pemesanan**:  
  - Daftar menu kopi dengan gambar, harga, dan deskripsi.  
  - Filter berdasarkan kategori (espresso, latte, dll.) atau harga.  
  - Fitur pencarian menu.  
- **Keranjang Belanja**:  
  - Tambah/edit/hapus item.  
  - Kustomisasi pesanan (contoh: tingkat kemanisan, tambahan topping).  
  - Perhitungan total otomatis termasuk pajak.  
- **Checkout & Pembayaran**:  
  - Pilih metode pembayaran (OVO/Gopay/Transfer Bank/Midtrans).  
  - Konfirmasi pembayaran otomatis (webhook).  
  - Notifikasi status pesanan (email/WhatsApp).  
- **Akun Pengguna**:  
  - Registrasi/login dengan email atau Google OAuth.  
  - Riwayat pesanan dan status pengiriman (jika ada delivery).  

### **2. Untuk Admin**  
- **Dashboard Analitik**:  
  - Grafik penjualan harian/bulanan.  
  - Menu paling laris dan pendapatan.  
- **Manajemen Menu**:  
  - CRUD menu (nama, harga, gambar, kategori, ketersediaan stok).  
  - Upload gambar dengan kompresi otomatis.  
- **Manajemen Pesanan**:  
  - Daftar pesanan masuk (status: diproses/selesai/dibatalkan).  
  - Konfirmasi pembayaran manual (jika diperlukan).  
- **Manajemen Pengguna**:  
  - Lihat daftar pelanggan.  
  - Reset password atau blokir akun.  

---

## **Teknologi yang Digunakan**  

### **Frontend**  
- **React.js** dengan **TypeScript** untuk type safety.  
- **Tailwind CSS** atau **Material-UI** untuk desain responsif.  
- **Redux Toolkit** untuk state management (keranjang, auth).  
- **Axios** untuk komunikasi API.  
- **React Router** untuk navigasi multi-halaman.  

### **Backend**  
- **Node.js** + **Express.js** untuk REST API.  
- **MongoDB** (NoSQL) dengan **Mongoose** (skema fleksibel untuk menu/pesanan).  
  - *Alternatif*: MySQL/PostgreSQL jika butuh relasional.  
- **JWT** untuk autentikasi.  
- **Multer** untuk upload gambar.  
- **Nodemailer** untuk notifikasi email.  

### **Integrasi Eksternal**  
- **Midtrans** atau **Xendit** untuk pembayaran digital.  
- **Firebase Storage** (jika butuh penyimpanan gambar eksternal).  
- **WhatsApp API** (Twilio) untuk notifikasi pesanan.  

### **DevOps**  
- **Docker** untuk containerisasi.  
- **CI/CD**: GitHub Actions atau Jenkins.  
- **Deployment**:  
  - Frontend: Vercel/Netlify.  
  - Backend: Heroku/Railway.  
  - Database: MongoDB Atlas/AWS RDS.  

---

## **Cara Instalasi**  

### **Prerequisites**  
- Node.js ≥ v18  
- MongoDB (local/Atlas)  
- Akun Midtrans/Xendit (opsional)  

### **Langkah-Langkah**  
1. Clone repositori:  
   ```bash
   git clone https://github.com/royhtml/coffie-shop.git
   cd coffie-shop
   ```

2. Setup Backend:  
   ```bash
   cd backend
   npm install
   cp .env.example .env  
   npm run dev
   ```

3. Setup Frontend:  
   ```bash
   cd ../frontend
   npm install
   npm start
   ```

4. Akses aplikasi di `http://localhost:3000`.

---

## **Kontribusi**  
- Laporkan bug atau permintaan fitur via **GitHub Issues**.  
- Ikuti panduan kode dan testing (Jest/RTL).  
- Branch naming: `feat/nama-fitur` atau `fix/nama-perbaikan`.  

---

## **Roadmap**  
- [ ] Tambahkan fitur loyalitas poin pelanggan.  
- [ ] Integrasi sistem delivery (Grab/Gojek API).  
- [ ] Aplikasi mobile (React Native/Flutter).  

---

## **Lisensi**  
Proyek ini open-source di bawah **MIT License**.  

---

**Catatan**:  
- Untuk demo langsung, sediakan link demo (contoh: [demo-coffie.vercel.app](https://demo-coffie.vercel.app)).  
- Jika proyek sudah live, tambahkan dokumentasi API (Swagger/Postman).  

Dengan detail ini, tim pengembang atau kontributor dapat memahami alur kerja dan skalabilitas proyek dengan lebih baik. 🚀

### **pengembang**

- Nama: Dwi Bakti Nur
- Github: dwidevelopes
- developers : dwi bakti n dev