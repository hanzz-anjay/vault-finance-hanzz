# Vault Finance Hanzz — starter project

## Isi paket
- `www/` : aplikasi web responsif/PWA (dashboard, transaksi, aset, reminder)
- `capacitor.config.json` dan `package.json` : konfigurasi awal untuk membungkus web menjadi aplikasi Android dengan Capacitor.

## Jalankan sebagai website/PWA
1. Upload folder `www` ke hosting HTTPS (mis. Vercel/Netlify).
2. Buka URL hosting di Chrome Android.
3. Pilih menu Chrome → **Install app** / **Tambahkan ke layar utama**.

## Membuat APK Android
Persyaratan: Node.js, Android Studio, Android SDK, dan koneksi internet.
1. Ekstrak ZIP.
2. Jalankan `npm install`.
3. Jalankan `npx cap add android`.
4. Jalankan `npx cap sync android`.
5. Jalankan `npx cap open android`.
6. Di Android Studio pilih Build → Build Bundle(s) / APK(s) → Build APK(s).

## Catatan penting
- Ini starter/prototipe lokal. Data disimpan di browser/perangkat menggunakan localStorage.
- Sinkronisasi HP-laptop belum aktif. Untuk itu perlu backend cloud (mis. Supabase), autentikasi, dan konfigurasi proyek.
- Pengingat tersimpan dalam aplikasi, tetapi notifikasi terjadwal saat aplikasi tertutup belum diaktifkan. Implementasi produksi perlu plugin notifikasi lokal/layanan penjadwalan dan izin Android.
- Nilai aset dimasukkan manual; aplikasi tidak terhubung ke bursa, exchange, atau harga pasar.
- Jangan masukkan PIN, password, seed phrase, atau kredensial keuangan ke prototipe ini.
