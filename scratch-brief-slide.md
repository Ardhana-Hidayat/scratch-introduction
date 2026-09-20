# Context Brief: Slide Interaktif "Mengenal Blok Kode di Scratch"

## Target
- Mata pelajaran: Informatika, SMP Kelas VIII
- Format output: single-file HTML dengan CSS + JS inline, navigasi antar slide (next/prev), bisa dijalankan langsung di browser tanpa server
- Gaya: playful tapi tetap rapi, warna-warna cerah sesuai kategori blok Scratch (motion=biru, looks=ungu, sound=magenta, events=kuning, control=oranye, sensing=cyan, operators=hijau, variables=oranye tua)

## Struktur Slide

1. **Cover**
   - Judul: "Mengenal Blok Kode di Scratch"
   - Subjudul: Materi Informatika Kelas 8 SMP
   - Elemen interaktif: beberapa blok Scratch palsu (dekoratif) yang bergoyang pelan (CSS animation) di background

2. **Apa itu Scratch?**
   - Bahasa pemrograman visual berbasis blok, dikembangkan MIT
   - Blok disusun seperti puzzle untuk animasi, game, cerita interaktif
   - Interaktif: animasi drag-and-drop sederhana (dua blok puzzle nyambung dengan efek "klik" saat di-drag mendekat) — bisa pakai JS pointer events, tidak perlu library

3. **Bagian Utama Scratch**
   - Stage, Sprite, Script Area, Block Palette
   - Interaktif: diagram/layout mirip tampilan asli Scratch, tiap bagian bisa di-hover/klik untuk munculkan tooltip penjelasan

4-11. **Satu slide per kategori blok** (Motion, Looks, Sound, Events, Control, Sensing, Operators, Variables)
   - Tiap slide: warna kategori konsisten, daftar blok dengan bentuk visual menyerupai blok Scratch asli (rounded, sesuai bentuk: hexagon untuk boolean/sensing kondisi, oval untuk reporter/operator angka, jigsaw untuk command)
   - Isi tiap blok: nama blok, contoh sintaks, penjelasan singkat (ambil dari dokumen sumber)
   - Interaktif: klik pada satu blok untuk expand/collapse penjelasan lebih detail, atau hover untuk highlight

12. **Contoh Program Sederhana**
   - Rangkaian 4 blok: when green flag clicked → move (10) steps → play sound [pop] until done → say [Halo!] for (2) seconds
   - Interaktif: tombol "Jalankan" yang memicu animasi simulasi sederhana (sprite emoji/ikon bergerak, muncul speech bubble "Halo!") pakai CSS transition/JS, sebagai simulasi visual hasil program

13. **Kesimpulan**
   - Ringkasan 3 poin dari materi sumber
   - Interaktif: quiz singkat 2-3 soal pilihan ganda (misal: "Blok mana yang termasuk kategori Events?") dengan feedback benar/salah langsung

## Kebutuhan Teknis
- Navigasi: tombol next/prev, indikator progress (dot atau nomor slide), bisa juga panah keyboard (arrow key) untuk pindah slide
- Semua CSS dan JS dalam satu file HTML (self-contained), tidak pakai library eksternal kecuali via CDN yang umum (opsional, boleh tanpa library sama sekali)
- Responsif untuk ditampilkan di proyektor (rasio 16:9) maupun dicoba di laptop siswa
- Font: jelas dan mudah dibaca dari jarak jauh (sans-serif, ukuran besar untuk judul)
- Setiap efek interaktif harus ringan dan tidak mengganggu alur presentasi (bukan permainan berat, hanya penguat pemahaman)

## Sumber Konten
Seluruh isi teks (definisi, nama blok, contoh sintaks, penjelasan fungsi) diambil langsung dari dokumen "Materi Informatika Kelas 8 SMP - Mengenal Blok Kode di Scratch" yang dilampirkan, tanpa mengubah maksud aslinya.