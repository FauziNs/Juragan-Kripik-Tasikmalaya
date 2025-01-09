# Juragan Kripik Tasikmalaya

## Deskripsi Proyek

**Juragan Kripik Tasikmalaya** adalah sebuah website statis yang dibangun menggunakan **HTML** dan **CSS** untuk mempromosikan produk camilan khas Tasikmalaya. Website ini menampilkan produk-produk terbaik, jam operasional, serta informasi kontak untuk pelanggan yang ingin membeli secara langsung atau online.

---

## Fitur Utama

1. **Desain Responsif**: Website dapat diakses dengan baik di berbagai perangkat (desktop, tablet, dan smartphone).
2. **Halaman Menu Produk**: Menampilkan berbagai produk camilan dengan informasi harga dan gambar.
3. **Formulir Kontak**: Pengguna dapat mengirimkan pesan atau pertanyaan melalui formulir kontak.
4. **Visual Menarik**: Menggunakan animasi CSS untuk meningkatkan pengalaman pengguna.

---

## Teknologi yang Digunakan

- **HTML5**: Struktur dan elemen halaman.
- **CSS3**: Desain, animasi, dan responsivitas.

---

## Instalasi

1. Clone repository ini ke komputer Anda:

   ```bash
   git clone https://github.com/FauziNs/JuraganKripikTasikmalaya.git
   ```

2. Buka file `index.html` di browser Anda.

---

## Animasi yang Ditambahkan
Berikut adalah animasi CSS yang diterapkan untuk membuat website lebih menarik:

1. **Fade-in Effect**: Elemen-elemen utama muncul dengan lembut saat halaman dimuat.
2. **Hover Animation**: Produk akan membesar atau memiliki efek bayangan saat kursor diarahkan.
3. **Button Animation**: Tombol akan berubah warna atau memiliki efek gelombang saat diklik.
4. **Scroll Animation**: Elemen muncul satu per satu saat pengguna menggulir halaman.
5. **Loading Animation**: Tambahkan animasi loading saat website pertama kali diakses.

---

## Contoh Animasi CSS
Tambahkan kode berikut ke file `style.css`:

```css
/* Fade-in Animation */
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Animasi untuk elemen utama */
.main-content {
  animation: fadeIn 1.5s ease-in-out;
}

/* Hover Animation untuk produk */
.product-card:hover {
  transform: scale(1.05);
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  transition: all 0.3s ease;
}

/* Button Animation */
button {
  position: relative;
  overflow: hidden;
}

button::after {
  content: '';
  position: absolute;
  top: 0;
  left: 50%;
  transform: translateX(-50%) scale(0);
  width: 200%;
  height: 200%;
  background: rgba(255, 255, 255, 0.2);
  border-radius: 50%;
  transition: transform 0.6s;
}

button:hover::after {
  transform: translateX(-50%) scale(1);
}

/* Scroll Animation */
@keyframes slideIn {
  from {
    opacity: 0;
    transform: translateX(-50px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

.scroll-element {
  opacity: 0;
  animation: slideIn 1s ease forwards;
}
```

---

## Cara Berkontribusi

1. Fork repository ini.
2. Buat branch fitur baru:
   ```bash
   git checkout -b nama-fitur-anda
   ```
3. Commit perubahan Anda:
   ```bash
   git commit -m "Menambahkan fitur baru"
   ```
4. Push branch Anda:
   ```bash
   git push origin nama-fitur-anda
   ```
5. Buat pull request di GitHub.

---

## Author

- **Fauzi Noor Syabani**  
  Developer dan Pemilik Proyek  
  [GitHub](https://github.com/FauziNs)

---

## License

Proyek ini dilisensikan di bawah [MIT License](LICENSE).
