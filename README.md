# Panduan Lengkap Web Galeri Foto Google Drive + GitHub Pages

Web ini menghubungkan folder Google Drive Anda ke website modern yang dihosting gratis di GitHub Pages.

---

## 📌 Langkah 1: Siapkan Folder Google Drive

1. Buka [Google Drive](https://drive.google.com).
2. Klik kanan pada folder foto Anda ➡️ Pilih **Bagikan (Share)** ➡️ **Bagikan**.
3. Di bagian **Akses umum (General access)**, ubah dari *Dibatasi (Restricted)* menjadi **"Siapa saja yang memiliki link" (Anyone with the link)** dengan peran **Pelihat (Viewer)**.
4. Klik **Salin link**. Linknya akan terlihat seperti ini:
   ```text
   https://drive.google.com/drive/folders/1aBcDeFgHiJkLmNoPqRsTuVwXyZ?usp=sharing
   ```
5. **Ambil Folder ID-nya**: Kodenya adalah bagian setelah `/folders/`:
   👉 `1aBcDeFgHiJkLmNoPqRsTuVwXyZ` *(Simpan kode ini)*.

---

## 🔑 Langkah 2: Buat Google Drive API Key (100% Gratis)

1. Buka [Google Cloud Console](https://console.cloud.google.com/).
2. Buat project baru (misal beri nama `Galeri Foto`).
3. Di menu pencarian atas, cari **"Google Drive API"** ➡️ Klik dan tekan tombol **Enable (Aktifkan)**.
4. Masuk ke tab **Credentials** di sebelah kiri ➡️ Klik **+ Create Credentials** ➡️ Pilih **API Key**.
5. Kunci API Anda akan muncul (contoh: `AIzaSyD...`).
6. Salin API Key tersebut *(Simpan kunci ini)*.

---

## 🚀 Langkah 3: Deploy Gratis ke GitHub Pages

1. Buka akun [GitHub](https://github.com) Anda.
2. Klik tombol **New** untuk membuat repository baru:
   - Nama repo: misalnya `galeri-foto`
   - Pilih: **Public**
   - Centang: *Add a README file*
   - Klik **Create repository**.
3. Di dalam repository baru tersebut, klik **Add file** ➡️ **Upload files**.
4. Drag dan drop file `index.html` ini ke sana, lalu klik **Commit changes**.
5. Masuk ke tab **Settings** di repository tersebut:
   - Klik menu **Pages** di kolom kiri.
   - Di bagian *Build and deployment* ➡️ *Branch*, ubah dari `None` menjadi **`main`** (folder `/root`).
   - Klik tombol **Save**.
6. Tunggu sekitar 1–2 menit, refresh halaman Settings Pages. Link website Anda akan muncul, contohnya:
   ```text
   https://username-anda.github.io/galeri-foto/
   ```

---

## ⚙️ Langkah 4: Hubungkan Web dengan Google Drive Anda

1. Buka link website GitHub Pages Anda.
2. Klik tombol **Konfigurasi** (ikon gear di pojok kanan atas):
   - Masukkan **Folder ID** Google Drive Anda.
   - Masukkan **Google Drive API Key** Anda.
   - Klik **Simpan & Sinkronkan**.
3. Selesai! Semua foto dan subfolder yang ada di Google Drive Anda akan langsung tampil di website.

### 💡 Cara Menambah Foto Baru:
Anda cukup buka Google Drive di HP atau Laptop, lalu upload foto seperti biasa. Foto akan langsung otomatis muncul di website tanpa perlu edit kode lagi!
