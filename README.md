

# Projek Baru - Sistem Informasi Aset (Laravel)

Deskripsi
---------
Aplikasi sederhana seputar informasi aset barang

Cara install / setup (Windows)
------------------------------
1. Buka PowerShell, arahkan ke folder proyek:
   ```
   cd C:\xampp_new\projek_baru
   ```

2. Install dependensi Composer:
   ```
   composer install
   ```

3. Salin file env dan generate app key:
   ```
   copy .env.example .env
   php artisan key:generate
   ```

4. Edit `.env` (atur DB_CONNECTION, DB_HOST, DB_PORT, DB_DATABASE, DB_USERNAME, DB_PASSWORD).

5. Jalankan migration dan seeder:
   ```
   php artisan migrate
   php artisan db:seed --class=BarangSeeder
   ```

6. Jika menambah model/seeder baru:
   ```
   composer dump-autoload
   ```

7. Salin gambar background (contoh):
   ```
   Copy-Item "C:\Users\user\Pictures\Gambar1.jpg" -Destination "C:\xampp_new\projek_baru\public\images\Gambar1.jpg" -Force
   ```

8. Jalankan aplikasi:
   ```
   php artisan serve
   ```
   Akses: http://127.0.0.1:8000 (atau sesuai konfigurasi XAMPP/VirtualHost)

Routes utama
------------
- GET  /register  → form registrasi
- POST /register  → proses registrasi
- GET  /login     → form login
- POST /login     → proses login
- POST /logout    → logout
- GET  /dashboard → dashboard (autentikasi required)

Screenshots / Demo
-----------------


https://github.com/user-attachments/assets/e86b8395-0bfc-4dbc-8be1-f830d42dadf2






Butuh saya tambahkan file screenshot contoh di repo atau otomatis update semua index.blade.php?
