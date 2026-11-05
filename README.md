Implementasi Halaman Achievement — Arcly

Buat halaman khusus pencapaian pada website "arcly.cyou" dengan route:

"/achievement"

Halaman ini berfungsi sebagai arsip pencapaian pribadi yang terdiri dari dua kategori utama: Certificates dan Gaming Achievements.

Jangan mengubah halaman Home atau bagian website lainnya. Integrasikan halaman ini ke sistem routing dan navigasi yang sudah tersedia.

1. Certificates

Tampilkan empat sertifikat berikut sebagai koleksi sertifikat pribadi:

1. OSINT Exposed — Certificate of Participation
   - Image: https://raw.githubusercontent.com/Arsenadev/vz/main/osint-exposed.png
2. Software Developer — Dicoding
   - Image: https://raw.githubusercontent.com/Arsenadev/vz/main/dicoding-software-developer.png
3. Introduction to Financial Literacy — Dicoding
   - Image: https://raw.githubusercontent.com/Arsenadev/vz/main/dicoding-financial-literacy.png
4. CSIRT DIY — Certificate of Appreciation
   - Image: https://raw.githubusercontent.com/Arsenadev/vz/main/csirt-diy-appreciation.jpg

Cara kerja Certificates

- Seluruh sertifikat harus ditampilkan menggunakan sistem stacked cards.
- Setiap kartu merepresentasikan satu sertifikat.
- Kartu harus memiliki interaksi yang smooth.
- Ketika kartu dipilih, tampilkan sertifikat dalam ukuran penuh agar seluruh informasi dapat dibaca.
- Sediakan cara untuk menutup tampilan preview dan kembali ke koleksi.
- Pastikan gambar tidak terpotong atau mengalami perubahan rasio yang tidak semestinya.
- Gunakan URL gambar asli yang sudah diberikan.

2. Gaming Achievements

Buat bagian khusus untuk pencapaian game Mobile Legends: Bang Bang.

Identitas game

- Game: Mobile Legends: Bang Bang
- Logo game:
  https://raw.githubusercontent.com/Arsenadev/vz/main/5ba3d73b381296e3b90bb963ad309798.jpg

Rank Achievement

- Achievement: High Rank
- Stars: 2.652
- Rank emblem:
  https://raw.githubusercontent.com/Arsenadev/vz/main/79741-removebg-preview.png

Tampilkan angka 2.652 dengan keterangan Stars, bukan Points.

Global Hero Rankings

Terdapat empat pencapaian global hero:

Ranking| Hero
#1| Granger
#2| Nolan
#48| Julian
#72| Ling

Gunakan logo global/title emblem berikut untuk seluruh pencapaian hero:

https://raw.githubusercontent.com/Arsenadev/vz/main/79719-removebg-preview.png

Setiap hero harus memiliki data terpisah yang mencakup:

- Nama hero.
- Posisi global.
- Logo global.
- Status pencapaian sebagai former global ranking.

Jangan mengarang informasi tambahan seperti season, win rate, match count, atau tanggal pencapaian yang belum tersedia.

3. Interaksi Gaming Achievements

- Logo Mobile Legends menjadi identitas utama kategori gaming.
- Rank achievement ditampilkan sebagai pencapaian tersendiri.
- Setiap global hero ranking memiliki kartu tersendiri.
- Sediakan tempat untuk screenshot bukti pencapaian masing-masing hero.
- Jika screenshot belum tersedia, jangan membuat bukti palsu atau menggunakan gambar hero sebagai bukti.
- Struktur data harus memudahkan penambahan screenshot bukti di kemudian hari.

4. Struktur dan Pengelolaan Data

Pisahkan data sertifikat dan gaming achievements agar mudah dikelola.

Hindari menulis data yang sama berulang kali.

Gunakan struktur data yang memungkinkan:

- Menambahkan sertifikat baru.
- Mengubah URL gambar sertifikat.
- Menambahkan hero baru.
- Mengubah ranking hero.
- Menambahkan screenshot bukti.
- Memperbarui jumlah Stars.

Semua gambar harus menggunakan URL yang sudah disediakan dan memiliki fallback apabila gagal dimuat.

5. Ketentuan Implementasi

- Periksa struktur project dan sistem routing yang sudah ada sebelum melakukan perubahan.
- Jangan merusak fitur yang sudah berjalan.
- Jangan membuat database baru. Seluruh data pencapaian cukup menggunakan data statis.
- Pastikan seluruh fitur berfungsi di perangkat mobile maupun desktop.
- Jangan mengarang data pribadi atau pencapaian.
- Pastikan preview sertifikat dan interaksi kartu dapat digunakan dengan baik.
- Lakukan pengecekan setelah implementasi dan perbaiki error yang ditemukan.