# Anak Emak Server Vote | Indonesia

Project siap pakai: sistem **vote server Minecraft** mirip konsep Minecraft-MP, khusus untuk server Indonesia.
Dirancang sebagai versi lengkap (pilihan B) termasuk halaman daftar, detail, voting dengan cooldown, admin panel untuk menambah server dan melihat votes.

## Cara jalankan (lokal)

1. Pastikan Node.js (v16+) terpasang.
2. Buka terminal di folder `backend`:
```bash
cd backend
npm install
node server.js
```
3. Buka browser: `http://localhost:3000`

Admin default disediakan saat pertama run:
- username: `admin`
- password: `adminpass`

Upload banner dan server via Admin > Tambah Server.

## Catatan
- Database SQLite disimpan di `backend/db.sqlite`.
- File upload banner disimpan di `frontend/public/uploads`.
- Untuk production, ganti `SESSION_SECRET` dan pertimbangkan migrasi ke PostgreSQL / managed DB, serta tambahkan CAPTCHA & rate rules.