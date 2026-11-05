# Panduan Menulis Berita — Berita Prodi BKI STAIFA

Setiap berita adalah **satu file** di folder `_posts`. Setelah file disimpan (*commit*), situs memperbarui diri sendiri dalam 1–2 menit.

## Menerbitkan berita baru

1. Buka repo di GitHub, lalu masuk ke folder **`_posts`**.
2. Klik **Add file → Create new file**.
3. Beri nama file dengan pola **`TAHUN-BULAN-TANGGAL-judul-singkat.md`**, misalnya:
   `2026-11-12-seminar-konseling-keluarga.md`
   - Gunakan huruf kecil dan tanda strip, tanpa spasi.
   - Tanggal di nama file menjadi tanggal terbit berita.
   - Jangan lupa akhiran **`.md`**.
4. Buka file **`TEMPLATE-BERITA.md`** di halaman utama repo, salin seluruh isinya, lalu tempel ke file baru.
5. Ganti isian di antara tanda `---` (bagian atas):

   | Baris | Isi |
   | --- | --- |
   | `title` | Judul berita, di antara tanda kutip |
   | `rubrik` | Salah satu dari: `kegiatan`, `pengumuman`, `prestasi`, `artikel` |
   | `ringkasan` | 1–2 kalimat rangkuman, di antara tanda kutip |
   | `gambar` | Alamat foto (lihat bagian foto). Hapus baris ini jika tidak ada foto |
   | `keterangan_gambar` | Keterangan foto. Hapus jika tidak ada foto |
   | `penulis` | Nama penulis. Hapus baris ini untuk memakai "Admin Prodi BKI" |

6. Tulis isi berita di bawah garis `---` kedua.
7. Klik **Commit changes…**, lalu **Commit changes**.
8. Tunggu centang hijau di tab **Actions**, lalu buka situs untuk melihat hasilnya.

Jika ada judul atau ringkasan yang memuat tanda kutip ("), ganti dengan tanda kutip tunggal (').

## Menambahkan foto

1. Kecilkan ukuran foto terlebih dahulu (lebar sekitar 1600 piksel, ukuran di bawah 500 KB) agar situs cepat dibuka.
2. Beri nama file foto tanpa spasi, misalnya `seminar-konseling-2026.jpg`.
3. Buka folder **`assets/img/berita`**, klik **Add file → Upload files**, unggah foto, lalu **Commit changes**.
4. Di berita, isi baris gambar dengan: `gambar: /assets/img/berita/seminar-konseling-2026.jpg`

Foto di tengah tulisan bisa ditambahkan dengan baris:
`![Keterangan foto](/berita/assets/img/berita/nama-foto.jpg)`

## Mengubah atau menghapus berita

- **Mengubah:** buka file berita di folder `_posts`, klik ikon pensil ✏️, ubah, lalu **Commit changes**.
- **Menghapus:** buka file berita, klik menu **⋯** di kanan atas, pilih **Delete file**, lalu **Commit changes**.

## Format teks

| Ditulis | Hasilnya |
| --- | --- |
| `**teks**` | **teks tebal** |
| `*teks*` | *teks miring* |
| `## Subjudul` | Subjudul |
| `- poin` | daftar poin |
| `1. langkah` | daftar bernomor |
| `[teks](https://…)` | tautan |
| `> kutipan` | kutipan |

## Jika berita tidak muncul

- Tanggal di nama file tidak boleh lebih dari hari ini, karena berita bertanggal masa depan tidak ditampilkan.
- Periksa nama file: harus diawali tanggal dan diakhiri `.md`.
- Periksa bagian atas: harus diawali dan ditutup baris `---`, dan setiap isian berbentuk `nama: isi`.
- Buka tab **Actions**. Jika ada tanda silang merah, klik untuk melihat pesan kesalahannya.
