# Audit Modul 2 - Semantic HTML dan Formulir

## Sebelum perbaikan

| Temuan | Halaman/elemen | Bukti | Rencana perbaikan |
|---|---|---|---|
| Katalog masih berupa ul/li | peralatan.html | DOM | Ubah menjadi section + article + figure |
| Form belum tersedia | peminjaman.html | file belum ada | Buat halaman baru dan form lengkap |
| Navigasi hanya 2 halaman | index.html, peralatan.html | DOM nav | Tambah link "Ajukan Peminjaman" |
| Footer masih menyebut "Proyek semester" | index.html | DOM footer | Ganti jadi teks latihan praktikum |

## Setelah perbaikan

- [x] Landmark halaman masuk akal (header, nav, main, section, footer).
- [x] Hierarki heading logis (h1 judul halaman, h2 judul kelompok katalog, h3 nama tiap alat).
- [x] Minimal tiga item katalog lengkap (Multimeter, Router, Kamera) dengan gambar, keterangan, stok, dan kondisi.
- [x] Label dapat diklik dan fokus berpindah ke kontrol yang benar (for cocok dengan id di semua field).
- [x] Field penting memiliki name (nim, nama, alat, tanggal_pinjam, durasi, keperluan, setuju).
- [x] Submit kosong memunculkan validasi browser (semua field wajib memakai required).
- [x] Urutan Tab logis: Navigasi -> NIM -> Nama lengkap -> Peralatan -> Tanggal peminjaman -> Durasi -> Keperluan -> Persetujuan -> Kirim pengajuan.
- [ ] Validator W3C Nu HTML Checker belum dijalankan (dicek manual saat internet tersedia).



## Refleksi singkat

- section, article, sama div itu bedanya di fungsi dan maknanya. section buat ngelompokin konten yang masih satu tema, article buat satu konten yang bisa berdiri sendiri, sedangkan div cuma buat pembungkus aja tanpa makna khusus.

- Placeholder hilang begitu pengguna mulai mengetik dan tidak terbaca oleh sebagian pembaca layar sebagai label permanen, sehingga tidak bisa menggantikan `<label>`.
- Atribut `name` akan menjadi kunci data yang dikirim ke backend saat form benar-benar diproses pada modul berikutnya; tanpa `name`, nilai field tidak ikut terkirim meski terlihat normal di browser.

- Pengujian keyboard menunjukkan pentingnya urutan HTML yang benar; jika urutan elemen di kode diacak, fokus akan terasa "loncat" walau tampilan visualnya tetap rapi.
- Starter Modul 2 tidak boleh menimpa repository Modul 1 karena akan menghapus riwayat commit dan hasil kerja sebelumnya; starter hanya dipakai sebagai referensi pembanding.
