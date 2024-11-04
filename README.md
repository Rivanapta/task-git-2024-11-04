# Golang Project

Tetaplah hidup walaupun tidak berguna heheh

## Created by : Rivan Apta Kusuma

# Panduan Membuat Repository Baru dan Melakukan Pull Request dengan Git Bash

Panduan ini akan membantu Anda membuat repository baru di GitHub, melakukan commit, push, dan membuat pull request menggunakan Git Bash.

## Langkah-langkah

### 1. **Membuat Repository Baru di GitHub**

   - Buka [GitHub](https://github.com) dan login ke akun Anda.
   - Klik tombol **New** atau ikon **+** di sudut kanan atas untuk membuat repository baru.
   - Isi nama repository, deskripsi (opsional), dan pilih visibilitas (Public atau Private).
   - Klik **Create repository**.

### 2. **Membuat Repository di Direktori Lokal dengan Git Bash**

   - Buka Git Bash dan navigasi ke direktori tempat Anda ingin menyimpan proyek:
     ```bash
     cd /path/to/your/directory
     ```
   - Inisialisasi repository Git di direktori tersebut:
     ```bash
     git init
     ```

### 3. **Menghubungkan Repository Lokal ke Repository GitHub**

   - Sambungkan repository lokal Anda ke repository di GitHub yang baru saja dibuat. Salin URL repository GitHub Anda, misalnya `https://github.com/username/repository-name.git`, dan jalankan:
     ```bash
     git remote add origin https://github.com/username/repository-name.git
     ```

### 4. **Menambahkan File dan Melakukan Commit**

   - Tambahkan file ke dalam repository lokal Anda:
     ```bash
     git add .
     ```
   - Buat commit awal:
     ```bash
     git commit -m "Initial commit"
     ```

### 5. **Push Commit ke Repository GitHub**

   - Kirim commit awal ke repository GitHub:
     ```bash
     git push -u origin main
     ```
   **Catatan**: Jika menggunakan branch `master`, ganti `main` dengan `master`.

### 6. **Membuat Branch Baru untuk Perubahan**

   - Buat branch baru untuk mengerjakan perubahan atau fitur baru:
     ```bash
     git checkout -b nama-branch
     ```
   - Lakukan perubahan pada file, lalu tambahkan perubahan ke staging area:
     ```bash
     git add .
     ```
   - Commit perubahan Anda:
     ```bash
     git commit -m "Deskripsi perubahan yang dibuat"
     ```

### 7. **Push Branch Baru ke GitHub**

   - Setelah commit selesai, push branch ke GitHub:
     ```bash
     git push origin nama-branch
     ```

### 8. **Membuat Pull Request di GitHub**

   - Buka repository di GitHub.
   - Anda akan melihat pesan untuk membuat pull request dari branch baru. Klik **Compare & pull request**.
   - Isi judul dan deskripsi pull request, lalu klik **Create pull request**.

### 9. **Merge Pull Request (Opsional)**

   - Setelah pull request ditinjau dan disetujui, Anda bisa menggabungkannya ke branch `main` dengan klik **Merge pull request**.
   - Jika tidak diperlukan lagi, Anda bisa menghapus branch setelah merge.

