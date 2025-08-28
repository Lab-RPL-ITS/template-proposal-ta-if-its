# Template LaTeX Proposal Tugas Akhir Departemen Teknik Informatika ITS

[![latest version](https://img.shields.io/github/v/release/Lab-RPL-ITS/template-proposal-ta-if-its)](https://github.com/Lab-RPL-ITS/template-proposal-ta-if-its/releases/)
[![commits since latest version](https://img.shields.io/github/commits-since/Lab-RPL-ITS/template-proposal-ta-if-its/latest)](https://github.com/Lab-RPL-ITS/template-proposal-ta-if-its/commits/master)
[![repo size](https://img.shields.io/github/repo-size/Lab-RPL-ITS/template-proposal-ta-if-its)](https://github.com/b201lab/template-buku-ta-its)
[![license](https://img.shields.io/github/license/Lab-RPL-ITS/template-proposal-ta-if-its)](./LICENSE)
[![build status](https://img.shields.io/github/actions/workflow/status/Lab-RPL-ITS/template-proposal-ta-if-its/ci.yml?branch=main)](https://github.com/Lab-RPL-ITS/template-proposal-ta-if-its/actions)

Repositori ini berisi template [LaTeX](https://www.latex-project.org/) lengkap untuk proposal tugas akhir yang disesuaikan dengan format resmi [Institut Teknologi Sepuluh Nopember](https://www.its.ac.id/) (ITS). Template ini dirancang untuk memenuhi standar akademik yang ditetapkan berdasarkan [SK Rektor ITS No. 280 Tahun 2022](https://www.its.ac.id/pendidikan/wp-content/uploads/sites/112/2022/03/280-SK-Rektor-ttg-Pedoman-Penyusunan-Laporan-Tugas-Akhir-Sarjana-Sarjana-Terapan.pdf) tentang pedoman penyusunan laporan tugas/proyek akhir program sarjana dan sarjana terapan.

Template ini mencakup semua komponen yang diperlukan untuk proposal tugas akhir, mulai dari sampul hingga jadwal penelitian, dengan format yang telah disesuaikan untuk berbagai departemen di ITS.

> Contoh file PDF dari template ini bisa dilihat di [sini](https://b201lab.github.io/template-proposal-ta-its/proposal-ta.pdf).

## Fitur

### Format dan Struktur Dokumen

- Format ukuran halaman A4, margin, dan font Times New Roman sesuai standar ITS
- Struktur dokumen lengkap dengan penomoran halaman yang benar (romawi untuk bagian awal, arab untuk isi)
- Template sampul bahasa Indonesia dan Inggris
- Lembar pengesahan dengan format resmi ITS
- Abstrak dalam bahasa Indonesia dan Inggris

### Komponen Proposal

- **Pendahuluan**: Latar belakang, rumusan masalah, batasan masalah, tujuan, dan manfaat
- **Tinjauan Pustaka**: Hasil penelitian terdahulu dan dasar teori dengan sistem referensi
- **Metodologi**: Metode penelitian, bahan dan alat, urutan pelaksanaan
- **Jadwal Penelitian**: Timeline penelitian dalam format tabel

### Fitur LaTeX Lanjutan

- Sistem referensi otomatis menggunakan BibLaTeX dengan style APA
- Penomoran gambar, tabel, dan persamaan secara otomatis
- Dukungan untuk code listings dengan syntax highlighting
- Pembuatan daftar isi, daftar gambar, daftar tabel, dan daftar kode sumber otomatis
- Dukungan format gambar JPEG, PNG, dan format lain
- Template tabel timeline dengan pewarnaan sel
- Formatting persamaan matematika yang rapi

### Automasi dan Tools

- Kompilasi dokumen secara otomatis menggunakan [GitHub Actions](https://github.com/features/actions)
- Pengaturan hyphenation bahasa Indonesia
- Sistem cross-reference untuk gambar, tabel, dan persamaan

## Cara Menggunakan Template

### 1. File Utama

File utama dokumen adalah [`main.tex`](./main.tex) yang mengatur:

- Package LaTeX yang digunakan
- Konfigurasi format dokumen (margin, font, spacing)
- Struktur dokumen dan urutan bab
- Styling untuk judul, referensi, dan numbering

### 2. Struktur Direktori dan File

#### 📁 [`konten/`](./konten) - Isi Proposal

Berisi file `.tex` untuk setiap bab proposal:

- `1-pendahuluan.tex` - Latar belakang, rumusan masalah, tujuan, manfaat
- `2-tinjauan-pustaka.tex` - Penelitian terdahulu dan dasar teori
- `3-metodologi.tex` - Metode penelitian dan tools yang digunakan
- `4-jadwal-penelitian.tex` - Timeline penelitian dalam format tabel

#### 📁 [`lainnya/`](./lainnya) - Komponen Tambahan

- `abstrak.tex` - Abstrak dalam bahasa Indonesia
- `abstrak-en.tex` - Abstrak dalam bahasa Inggris
- `lembar-pengesahan.tex` - Halaman pengesahan resmi
- `lembar-pengesahan-en.tex` - Halaman pengesahan bahasa Inggris

#### 📁 [`sampul/`](./sampul) - Halaman Sampul

- `konten-id.tex` - Konten sampul bahasa Indonesia
- `konten-en.tex` - Konten sampul bahasa Inggris
- `sampul-luar.tex` - Template layout sampul
- `gambar/sampul-luar-tipis.png` - Logo dan elemen visual sampul

#### 📁 [`pustaka/`](./pustaka) - Referensi

- `pustaka.bib` - Database referensi dalam format BibTeX
- `tanda-hubung.tex` - Pengaturan hyphenation bahasa Indonesia

#### 📁 [`gambar/`](./gambar) - Aset Visual

Tempat menyimpan gambar, diagram, dan ilustrasi dalam format `.jpg`, `.png`, atau format lain

### 3. Langkah Penggunaan

1. **Personalisasi Data**: Edit informasi mahasiswa, dosen pembimbing, dan judul di file sampul dan abstrak
2. **Isi Konten**: Lengkapi setiap file di direktori `konten/` sesuai penelitian Anda
3. **Tambah Referensi**: Masukkan referensi ke `pustaka/pustaka.bib` dalam format BibTeX
4. **Tambah Gambar**: Simpan gambar di direktori `gambar/` dan referensikan di konten
5. **Kompilasi**: Jalankan LaTeX compiler untuk menghasilkan `main.pdf`

### 4. Tips Penggunaan

- Setiap file dilengkapi dengan komentar panduan penggunaan
- Gunakan label dan reference untuk cross-referencing otomatis
- Format sitasi menggunakan `\parencite{}` untuk referensi dalam teks
- Gunakan environment `figure`, `table`, dan `equation` untuk elemen yang perlu dinomori

> Penjelasan lengkap dan contoh penggunaan tersedia dalam komentar di setiap file template.

## Persyaratan Sistem

### LaTeX Distribution

Template ini memerlukan distribusi LaTeX yang lengkap seperti:

- **TeX Live** (Linux/Windows/macOS) - Rekomendasi
- **MiKTeX** (Windows)
- **MacTeX** (macOS)

### Package Dependencies

Template menggunakan package LaTeX berikut:

- `geometry` - pengaturan margin dan ukuran halaman
- `setspace` - pengaturan spasi baris
- `biblatex` - manajemen referensi dengan style APA
- `graphicx` - dukungan gambar
- `hyperref` - hyperlink dan bookmark PDF
- `listings` - code syntax highlighting
- `algorithm2e` - formatting algoritma
- `tocloft` - custom table of contents
- `titlesec` - custom section formatting

### Kompilasi

Untuk menghasilkan dokumen PDF:

```bash
pdflatex main.tex
```

Atau gunakan `latexmk` untuk kompilasi otomatis:

```bash
latexmk -pdf main.tex
```

## Kontribusi

Kontribusi untuk pengembangan template ini sangat diterima. Silakan:

1. Fork repositori ini
2. Buat branch untuk fitur baru (`git checkout -b feature/nama-fitur`)
3. Commit perubahan (`git commit -am 'Menambah fitur baru'`)
4. Push ke branch (`git push origin feature/nama-fitur`)
5. Buat pull request

## Lisensi

Template ini dilisensikan di bawah [Lisensi MIT](./LICENSE). Anda bebas menggunakan, memodifikasi, dan mendistribusikan template ini untuk keperluan akademik maupun komersial.
