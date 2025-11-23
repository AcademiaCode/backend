# AcademiaCode - Backend API ⚙️

<div align="center">
  <img src="https://github.com/AcademiaCode/.github/blob/main/Icon.png?raw=true" alt="AcademiaCode Logo" width="100">
  <br>
  <strong>Server-side Logic & Database Management</strong>
  <br>
  <a href="https://academiacode-be.vercel.app/docs"><strong>📚 Dokumentasi Swagger API</strong></a>
</div>

---

## 📋 Tentang Modul Ini
Repository ini berisi *source code* untuk sisi server (Backend) dari ekosistem **AcademiaCode**. Modul ini bertanggung jawab menangani logika bisnis, autentikasi pengguna, manajemen database, serta integrasi dengan Piston API untuk eksekusi kode.

---

## 🏗️ Arsitektur & Desain Sistem

Untuk memahami bagaimana sistem ini bekerja di balik layar, berikut adalah diagram teknisnya:

### 1. Arsitektur Sistem
Gambaran besar bagaimana Client, Server, Database, dan Compiler Engine (Piston) saling berinteraksi.
![System Architecture](https://github.com/AcademiaCode/.github/blob/main/arsitektur_sistem.jpg?raw=true)

### 2. Class Diagram (Database Schema)
Struktur relasi database yang digunakan (User, Problem, Submission, Discussion, dll).
![Class Diagram](https://github.com/AcademiaCode/.github/blob/main/class_diagram.jpg?raw=true)

---

## 🛠️ Tech Stack (Backend)
* **Runtime:** Node.js & Express.js
* **Database:** PostgreSQL
* **ORM:** Prisma
* **Auth:** JWT (JSON Web Token)
* **Docs:** Swagger UI

---

## 🚀 Cara Menjalankan (Local Development)

1.  **Clone Repository & Install Dependencies**
    ```bash
    git clone [https://github.com/AcademiaCode/backend.git](https://github.com/AcademiaCode/backend.git)
    cd backend
    npm install
    ```

2.  **Konfigurasi Environment**
    Buat file `.env` dan sesuaikan variabel berikut:
    ```env
    DATABASE_URL="postgresql://user:password@localhost:5432/academiacode"
    JWT_SECRET="rahasia_super_aman"
    PORT=3000
    ```

3.  **Setup Database (Prisma)**
    ```bash
    npx prisma migrate dev --name init
    ```

4.  **Jalankan Server**
    ```bash
    npm run dev
    ```
    Server berjalan di `http://localhost:3000`

---
<div align="center">
  Bagian dari organisasi <a href="https://github.com/AcademiaCode"><strong>AcademiaCode</strong></a>.
</div>
