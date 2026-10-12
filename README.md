# Praktikum 4: CSS Layout (Box Element & Layout Sederhana) - Pemrograman Web
Repository ini dibuat untuk menyelesaikan tugas Praktikum 4 Pemrograman Web.

## Identitas Mahasiswa

| Keterangan      | Data                 |
| --------------- | -------------------- |
| **Nama**        | Rafli Putra Sudrajat |
| **Kelas**       | I251B                |
| **NIM**         | 312510326            |
| **Mata Kuliah** | Pemrograman Web      |
| **Dosen**       | Agung Nugroho, S.Kom., M.Kom. |

### Tujuan Praktikum

Mahasiswa mampu memahami konsep box element pada CSS (float dan clearfix).

Mahasiswa mampu membuat layout website sederhana menggunakan semantic element HTML5.

Mahasiswa mampu mengatur navigasi, hero panel, main content, sidebar, dan footer menggunakan CSS.

Mahasiswa mampu membuat halaman tambahan (About dan Kontak) dengan layout yang konsisten.

---

## Struktur Folder Proyek

```
Lab4Web/
├── Lab4_Layout/
│   ├── Lab4_Layout.html
│   ├── about.html
│   ├── kontak.html
│   └── style.css
├── Lab4web/
│   └── Lab4_box.html
└── README.md
```

<!-- Ganti dengan screenshot struktur folder -->

<img width="191" height="279" alt="image" src="https://github.com/user-attachments/assets/d816badb-1c07-4a8d-9a3f-8668b4719ae7" />


---

## Langkah-langkah Praktikum

### 1. Membuat Box Element (`Lab4_box.html`)

Langkah pertama adalah menyiapkan dokumen HTML dasar dengan nama `Lab4_box.html` yang berisi `<header>` dengan judul "Box Element".

<img width="906" height="370" alt="image" src="https://github.com/user-attachments/assets/dd6fb76c-150c-47cc-b29f-209c79f9f81e" />


Kemudian di dalam `<body>` ditambahkan `<section>` yang berisi empat buah `<div>` dengan class `div1` sampai `div4`.

<img width="423" height="151" alt="image" src="https://github.com/user-attachments/assets/30f6c439-2238-4054-b00f-be4f4164d944" />


#### CSS Float Property

Pada bagian `<head>` ditambahkan CSS internal untuk membuat float element:

- Semua `div` diberi `float: left` dan `padding: 10px`.
- `.div1` berwarna merah, `.div2` kuning, `.div3` hijau.
- `.div4` berwarna biru dengan `clear: left` dan `float: none` (clearfix) agar tampil di baris baru.

<img width="306" height="352" alt="image" src="https://github.com/user-attachments/assets/806fdb07-e6a1-474f-b36e-dbcfba87168d" />


Hasil di browser: Div1, Div2, dan Div3 tampil sejajar ke samping, sedangkan Div4 berada di bawahnya dengan lebar penuh.

<img width="610" height="329" alt="image" src="https://github.com/user-attachments/assets/5fb3c7e9-e158-4135-9f90-82e02386dc3c" />


---

### 2. Membuat Layout Sederhana (`Lab4_Layout.html`)

Membuat kerangka layout menggunakan semantic element. Dokumen ini menghubungkan file `style.css` dan memiliki `<div id="container">` sebagai pembungkus utama.

<img width="736" height="188" alt="image" src="https://github.com/user-attachments/assets/1a4aa22d-9185-41d6-903d-7dac1e0a90ac" />


Di dalam container ditambahkan elemen `<header>`, `<nav>` (Home, Artikel, About, Kontak), `<section id="hero">`, `<section id="wrapper">` (berisi `<section id="main">` dan `<aside id="sidebar">`), serta `<footer>`.

<img width="352" height="178" alt="image" src="https://github.com/user-attachments/assets/4bbf886c-7e86-45d3-8a45-87f9c89378f5" />

<img width="499" height="332" alt="image" src="https://github.com/user-attachments/assets/db698d27-dc9f-47be-8105-1871dd4b0b60" />



Hasil sebelum diberi CSS:

<img width="499" height="227" alt="image" src="https://github.com/user-attachments/assets/e732dd22-b7c0-48b7-abe8-4a1cff3e2c5b" />


---

### 3. Menambahkan CSS Layout (`style.css`)

CSS ditambahkan untuk membuat tampilan dasar layout, meliputi:

- `@import` Google Font **Open Sans** dan **Open Sans Condensed**.
- Reset CSS (`margin: 0; padding: 0`).
- Pengaturan `body` (font-size, font-family, warna teks).
- `#container` dengan lebar `980px`, rata tengah (`margin: 0 auto`), dan `box-shadow`.
- Pengaturan `header` dan `header h1`.

<img width="975" height="441" alt="image" src="https://github.com/user-attachments/assets/037b3cbe-949b-4b93-b855-9f124619cca8" />


Hasil di browser:

<img width="959" height="262" alt="image" src="https://github.com/user-attachments/assets/0325dff5-b0eb-49f2-a9b3-1c3a03af7b69" />


---

### 4. Mengatur Navigasi

CSS navigasi dibuat dengan ketentuan:

- `nav` memiliki background biru (`#1f5faa`).
- Link `nav a` ditampilkan `inline-block`, berwarna putih, tebal, tanpa garis bawah.
- `nav a.active` dan `nav a:hover` memiliki background `#2b83ea`.

<img width="314" height="342" alt="image" src="https://github.com/user-attachments/assets/56dded7f-4657-4a86-bdb0-850178644431" />


<img width="752" height="240" alt="image" src="https://github.com/user-attachments/assets/fc16e22a-90f6-4866-b155-4190e529a3b0" />


---

### 5. Membuat Hero Panel

Menambahkan kode HTML pada `<section id="hero">` berisi judul, paragraf, dan tombol "Learn more", lalu diberi style: background abu-abu (`#e4e4e5`), padding, serta pengaturan ukuran font `h1` dan `p`.

<img width="975" height="179" alt="image" src="https://github.com/user-attachments/assets/49dffe1e-dc0e-427b-9c0c-e17684d2d58e" />

<img width="253" height="251" alt="image" src="https://github.com/user-attachments/assets/8e0451d6-95e1-4785-9110-a50360e1f9fc" />


<img width="440" height="254" alt="image" src="https://github.com/user-attachments/assets/584c4f57-aa78-450f-897b-c47056ad9927" />


---

### 6. Menambahkan CSS Float untuk Main Content dan Sidebar

- `#main` dan `#sidebar` menggunakan `float: left`.
- Lebar `#main` = `640px`, lebar `#sidebar` = `260px`, keduanya dengan `padding: 20px`.
- Sidebar berisi dua `widget-box` (daftar link dan teks) yang diberi style border, title berwarna biru (`#428bca`), list tanpa bullet, dan efek hover.

<img width="202" height="294" alt="image" src="https://github.com/user-attachments/assets/3fda7fd2-57e1-420b-b54b-f825e85a3603" />


<img width="636" height="262" alt="image" src="https://github.com/user-attachments/assets/81c697d1-0f1e-41e6-a39e-723f717498c8" />


<img width="241" height="405" alt="image" src="https://github.com/user-attachments/assets/f6377fc5-7803-45a0-887e-78ae56c6da0b" />

<img width="361" height="413" alt="image" src="https://github.com/user-attachments/assets/86ef685a-47ed-43b1-b265-9b225c4bf1d4" />


---

### 7. Mengubah Tampilan Footer

Footer diberi style background gelap dengan teks putih agar terlihat berbeda dari konten utama.

<img width="609" height="73" alt="image" src="https://github.com/user-attachments/assets/b37f8ab1-e2fa-404e-872e-1833820bd3db" />


---

### 8. Menambahkan Elemen Lain pada Main Content

Menambahkan `div.row` yang berisi tiga `div.box`. Masing-masing box memiliki gambar, heading, paragraf, dan tombol "View detail". CSS yang digunakan:

- `.box` dengan `float: left`, `width: 33.333333%`, `box-sizing: border-box`, dan `text-align: center`.
- `.image-circle` dengan `border-radius: 50%` agar gambar berbentuk lingkaran.
- `.row` dengan margin negatif dan clearfix (`:before` dan `:after` dengan `display: table` dan `clear: both`).

<img width="688" height="305" alt="image" src="https://github.com/user-attachments/assets/06daaee8-e563-45fe-b162-a18299323335" />

<img width="358" height="445" alt="image" src="https://github.com/user-attachments/assets/21f2dc3e-94ea-495a-b4cd-719a5525250a" />
<img width="304" height="304" alt="image" src="https://github.com/user-attachments/assets/b268de0a-2587-454e-bd9c-6db9c3793c9f" />
<img width="322" height="272" alt="image" src="https://github.com/user-attachments/assets/26d56f2f-edb4-4cf1-b944-71b15aea41a8" />


---

### 9. Membuat Content Artikel

Menambahkan dua `<article class="entry">` yang dipisah dengan `<hr class="divider">`. Artikel pertama memiliki gambar di kiri, sedangkan artikel kedua memakai class `right-img` sehingga gambar berada di kanan.

CSS `.entry`:
- `margin: 15px 0`, `h2` dengan `margin-bottom: 20px`, dan `p` dengan `line-height: 25px`.
- `.entry img` menggunakan `float: left`, `border-radius: 5px`, dan `margin-right: 15px`.
- `.entry .right-img` menggunakan `float: right` dengan margin kiri `15px`.

<img width="578" height="248" alt="image" src="https://github.com/user-attachments/assets/19ff8570-955d-47e1-aa65-10052dccbc5c" />


<img width="244" height="376" alt="image" src="https://github.com/user-attachments/assets/25ac8edb-f782-4d35-8a59-0a75fc69fb66" />


<img width="469" height="316" alt="image" src="https://github.com/user-attachments/assets/cce429ae-882d-4f25-9c75-d7394e306fa7" />


---

## Pertanyaan dan Tugas

### 1. Menambahkan Menu About (`about.html`)

Membuat halaman About dengan layout yang sama (header, nav, hero, main, footer). Halaman ini berisi bagian **Tentang Saya** (hero), **Deskripsi Diri**, dan **Portfolio** (Website Layout Sederhana, Desain UI/UX, dan Project Pemrograman). Menu "About" diberi `class="active"`.

<img width="318" height="360" alt="image" src="https://github.com/user-attachments/assets/d0a18ba7-371d-437d-83f3-2926aca903a2" />

<img width="319" height="350" alt="image" src="https://github.com/user-attachments/assets/41a2a1d9-1ded-4b65-b1e1-2a50b4b4ccea" />

<img width="442" height="424" alt="image" src="https://github.com/user-attachments/assets/d1b49683-9411-4d34-9434-634eaef78112" />


### 2. Menambahkan Menu Kontak (`kontak.html`)

Membuat halaman Kontak yang berisi **Form Contact** dengan field Nama Lengkap, Email, Subjek, dan Pesan (textarea), serta tombol "Kirim Pesan". Semua field menggunakan atribut `required`, dan menu "Kontak" diberi `class="active"`.

<img width="362" height="714" alt="image" src="https://github.com/user-attachments/assets/67c5cce6-1bb0-4485-b760-d88edbba4f6e" />


<img width="474" height="486" alt="image" src="https://github.com/user-attachments/assets/1d9dce85-d375-46b1-a9ce-dd9a5cca348b" />


---

## Kesimpulan

Pada praktikum ini telah dipelajari cara membuat layout website dengan CSS menggunakan properti `float` dan `clear`, penggunaan semantic element HTML5, serta pembuatan komponen seperti navigasi, hero panel, sidebar widget, box, dan artikel. Selain itu juga dibuat halaman About dan Kontak dengan layout yang konsisten.
