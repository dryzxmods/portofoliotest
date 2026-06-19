# Portfolio Pertama - Irfan Sabrian

Repository ini berisi portfolio pertama Irfan Sabrian. Website ini dibuat sebagai halaman personal untuk menampilkan profil, layanan, pengalaman, project, CV, dan kontak.

## Ringkasan

Portfolio ini berbentuk static website satu halaman. Semua tampilan utama berada di `index.html`, styling tambahan berada di `css/style.css`, sedangkan interaksi halaman dikelola melalui file JavaScript di folder `js`.

Bagian utama website:

- Hero section dengan perkenalan singkat.
- Animasi typed text untuk role seperti Frontend Developer, Web Designer, GIS Enthusiast, dan Data Analytics Explorer.
- Section services untuk layanan/kemampuan.
- Timeline pengalaman dan pendidikan.
- Section projects dengan filter kategori dan pagination.
- Modal preview CV berbasis PDF.js.
- Contact form dengan `mailto`.
- Dark mode toggle.
- Responsive mobile menu.

## Teknologi

- HTML5.
- CSS3.
- JavaScript.
- Tailwind CSS via CDN.
- Font Awesome.
- Google Fonts.
- AOS Animate on Scroll.
- Typed.js.
- Particles.js.
- PDF.js untuk preview CV.

## Struktur Folder

```text
.
|-- assets/
|   |-- images/       # Logo, foto profil, dan thumbnail project
|   `-- pdf/          # File CV
|-- css/
|   `-- style.css     # Styling custom
|-- js/
|   |-- main.js       # Interaksi utama, dark mode, animasi, modal CV, contact form
|   `-- projects.js   # Data project, filter, pagination, dan render kartu project
|-- index.html        # Halaman utama portfolio
`-- README.md
```

## Fitur

- Desain landing page personal yang responsif.
- Navbar fixed dengan efek scroll.
- Mode terang dan gelap menggunakan `localStorage`.
- Hero section dengan efek partikel.
- Animasi teks role menggunakan Typed.js.
- Kartu project dinamis dari data JavaScript.
- Filter project berdasarkan kategori.
- Pagination project.
- Preview CV langsung di dalam modal.
- Tombol download CV.
- Contact form yang membuka email client melalui `mailto`.

## Cara Menjalankan

Karena project ini static website, cukup buka file:

```text
index.html
```

Atau jalankan dengan local server agar path aset lebih stabil.

Contoh menggunakan VS Code Live Server:

```text
Open with Live Server
```

Contoh menggunakan Python:

```bash
python -m http.server 8000
```

Lalu buka:

```text
http://localhost:8000
```

## Mengubah Data Project

Data project berada di:

```text
js/projects.js
```

Tambahkan object baru ke array `projects` dengan format seperti ini:

```js
{
  id: 5,
  title: "Nama Project",
  description: "Deskripsi singkat project",
  categories: ["web"],
  image: "assets/images/project.jpg",
  technologies: ["HTML", "CSS", "JavaScript"],
  links: {
    github: "https://github.com/username/repository",
    live: "https://domain-project.com"
  }
}
```

## Mengubah CV

File CV berada di:

```text
assets/pdf/CV_Irfan Sabrian Fadhillah.pdf
```

Jika nama file CV diganti, sesuaikan juga path di `js/main.js` pada bagian modal CV.

## Deployment

Project ini bisa dideploy ke layanan static hosting seperti GitHub Pages, Vercel, Netlify, atau hosting biasa. Pastikan semua file di repository ikut ter-upload agar gambar, logo, JavaScript, CSS, dan PDF CV tetap terbaca.
