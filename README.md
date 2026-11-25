# Portofolio — Ganistian Ridhotillah

Website portofolio satu halaman untuk menampilkan karya dan pengalaman belajar di jurusan **Desain Komunikasi Visual (DKV)**, SMKN 10 Surabaya.

Fokus: **Interface Design & User Research** — dibangun dengan HTML, Tailwind CSS (CDN), dan JavaScript vanilla, tanpa proses build.

![Preview halaman utama](assets/preview-hero.jpg)

[Lihat preview halaman penuh →](assets/preview-full.jpg)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38BDF8?style=flat-square&logo=tailwindcss&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![License: MIT](https://img.shields.io/badge/License-MIT-8E84E8?style=flat-square)

---

## Tentang

Portofolio ini berisi kumpulan tugas dan dokumentasi magang selama menempuh pendidikan di DKV:

- **Nirmana** — latihan komposisi, garis, titik, bentuk, warna, dan keseimbangan visual.
- **Poster / Feed Instagram** — latihan menyampaikan pesan secara komunikatif dan menarik.
- **Magang** — pengalaman menerapkan ilmu desain langsung di dunia kerja.

Desain memakai tema **dark navy + periwinkle** dengan grid teknis halus, tipografi *Plus Jakarta Sans*, dan aksen pill. Detail lengkap design system ada di [`DESIGN.md`](DESIGN.md).

## Fitur

- **Single page** dengan navigasi anchor: Home, Projects, About me, Contact.
- **Galeri karya** 2 grup (Nirmana & Magang) dengan 6 kartu project.
- **Modal preview project** — klik kartu untuk melihat detail, dengan tombol Prev/Next.
- **Keyboard support** — `Esc` menutup modal, `←` / `→` berpindah project.
- **Copy to clipboard** untuk WhatsApp, Instagram, telepon, dan email.
- **Responsif** — layout 2 kolom di desktop, 1 kolom di mobile.
- **Aksesibel** — touch target minimal 44×44 px, focus ring, `aria-label`, dan `role="dialog"` pada modal.
- **Tanpa build step** — cukup satu file `index.html`.

## Teknologi

| Bagian | Keterangan |
| --- | --- |
| Markup & style | HTML5, Tailwind CSS via CDN |
| Interaksi | JavaScript vanilla (modal, navigasi project, copy) |
| Font | Plus Jakarta Sans + Material Symbols (Google Fonts) |
| Ikon | Material Symbols Outlined |
| Hosting | GitHub Pages (static) |

## Struktur Proyek

```
portofolio-ganis/
├── index.html              # Halaman utama (markup, style, dan script)
├── DESIGN.md               # Dokumentasi design system (warna, tipografi, spacing)
├── assets/
│   ├── preview-hero.jpg    # Gambar preview untuk README
│   └── preview-full.jpg    # Preview halaman penuh
├── hero-profile.png        # Foto profil di hero
├── nirmana 1.jpeg          # Nirmana garis Flora
├── nirmana 2.jpeg          # Nirmana titik
├── nirmana 3.jpeg          # Nirmana garis Fauna
├── poster 3.jpeg           # Feed Instagram — magang ITS
├── magang 1.jpeg           # Magang Pertama — Kelir Advertising
├── magang 2.jpeg           # Magang 2 — PRODES ITS
├── logo 1.jpg              # Ikon Adobe Illustrator
├── logo 2.jpg              # Ikon Canva
├── logo 3.jpg              # Ikon Adobe Photoshop
├── LICENSE                 # Lisensi MIT
├── .gitignore
└── .nojekyll               # Mencegah GitHub Pages memproses file dengan Jekyll
```

> `screen.png`, `poster 1.jpeg`, dan `poster 2.jpeg` adalah arsip dan tidak dipakai oleh halaman. Boleh dihapus kalau tidak diperlukan.

## Menjalankan Secara Lokal

**Cara paling cepat:** klik dua kali `index.html` — halaman langsung terbuka di browser.

Atau jalankan local server (opsional):

```bash
# Python 3
python -m http.server 8000

# atau Node.js
npx serve .
```

Lalu buka <http://localhost:8000>.

> Koneksi internet diperlukan untuk memuat Tailwind CDN, Google Fonts, dan Material Symbols.

## Upload ke GitHub (via Web)

1. Buat repository baru di [github.com/new](https://github.com/new).
   - Isi **Repository name**, misalnya `portofolio-ganis`.
   - Pilih **Public**.
   - **Jangan** centang "Add a README file" — README sudah ada di folder ini.
2. Klik **Create repository**.
3. Di halaman repo, klik **Add file → Upload files**.
4. Drag & drop **semua isi folder** ini (termasuk folder `assets/`) ke area upload, lalu klik **Commit changes**.
   - Jika `.gitignore` / `.nojekyll` tidak ikut ter-upload, buat lewat **Add file → Create new file** dengan nama persis `.gitignore` dan `.nojekyll`.
5. Setelah file masuk, buka **Settings → Pages**.
6. Pada **Build and deployment → Source**, pilih **Deploy from a branch**.
7. Pilih branch **main** dan folder **/ (root)**, lalu **Save**.
8. Tunggu 1–2 menit. Situs tersedia di:

   ```
   https://<username>.github.io/<nama-repo>/
   ```

## Kustomisasi

| Yang ingin diubah | Lokasi |
| --- | --- |
| Nama, tagline, deskripsi | `index.html` — bagian `<!-- 1. Hero -->` |
| Judul & deskripsi project di modal | `index.html` — array `projectsData` di dalam `<script>` |
| Gambar project | ganti file `nirmana *.jpeg`, `poster 3.jpeg`, `magang *.jpeg` |
| Kontak | `index.html` — bagian `<!-- Right Column: Contact -->` (link `wa.me`, `instagram.com`, `tel:`, `mailto:` dan teks tombol copy) |
| Warna & tipografi | `DESIGN.md` + blok `tailwind.config` di `<head>` |
| Foto profil | ganti `hero-profile.png` |

**Penting:** urutan gambar di dalam `#projects` harus sama dengan urutan `projectsData`, karena modal mengambil gambar ke-N dari daftar `#projects img`.

## Catatan Teknis

- **Tailwind CDN** (`cdn.tailwindcss.com`) praktis untuk prototipe, tetapi memunculkan peringatan di console dan bukan rekomendasi resmi untuk produksi. Untuk versi produksi, gunakan Tailwind CLI dan hasilkan file CSS statis.
- **Satu gambar modal** masih memakai URL eksternal `lh3.googleusercontent.com` sebagai placeholder. Sebaiknya ganti dengan aset lokal agar tidak bergantung pada layanan pihak ketiga.
- **Nama file gambar memakai spasi** dan di-encode menjadi `%20` di HTML. Kalau ingin lebih rapi, rename ke kebab-case (mis. `nirmana-1.jpeg`) lalu sesuaikan `src`.
- Semua halaman bersifat statis — tidak ada backend, database, atau form yang mengirim data.

## Kontak

- **WhatsApp / Telepon:** 085606657347
- **Instagram:** [@spageti_mafiaw](https://instagram.com/spageti_mafiaw)
- **Email:** [ridhotillahganistian@gmail.com](mailto:ridhotillahganistian@gmail.com)

## Lisensi

Kode pada proyek ini dilisensikan di bawah [MIT License](LICENSE).

Karya visual di dalamnya (foto, gambar Nirmana, poster, dan logo) adalah hak cipta **Ganistian Ridhotillah** dan tidak tercakup dalam lisensi MIT. Mohon jangan menggunakan karya visual tanpa izin.

---

© 2025 Ganistian Ridhotillah — UI/UX Designer, SMKN 10 Surabaya
