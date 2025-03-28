# Portfolio Website - Bayu Adhi Nugroho

Pada tujuan pembuatan web ini yaitu untuk membuat web yang berisikan data diri saya. Tujuan pembuatan web ini yaitu agar mempermudah orang mengenali saya.

## 🚀 Fitur Utama

1. **Dark Mode Toggle**
   - Fitur untuk mengalihkan tampilan antara mode terang dan gelap
   - Menggunakan localStorage untuk menyimpan preferensi pengguna
   - Tombol "Mode Malam" untuk beralih antar mode

2. **Responsive Layout**
   - Desain yang menyesuaikan dengan berbagai ukuran layar
   - Media queries untuk pengalaman pengguna yang lebih baik di perangkat mobile
   - Struktur grid untuk menampilkan proyek portfolio

3. **Multi-Page Navigation**
   - Halaman terpisah untuk Home, About, Portfolio, dan Contact
   - Navigasi yang konsisten di semua halaman melalui navbar
   - Transisi halaman yang lancar

4. **Profil Diri**
   - Menampilkan foto profil dengan format circular
   - Bagian "About Me" yang berisi informasi singkat
   - Daftar keterampilan (HTML, CSS, JavaScript, SQL)

5. **Portfolio Showcase**
   - Tampilan grid untuk menampilkan proyek
   - Format kartu untuk setiap proyek
   - Link untuk detail proyek

6. **Contact Section**
   - Tautan ke platform media sosial (Instagram, Discord)
   - Desain tombol yang menarik dengan efek hover
   - Tata letak yang bersih dan mudah diakses

7. **CSS Transitions**
   - Efek hover pada tombol dan link
   - Transisi warna yang halus saat beralih mode
   - Animasi transform pada link sosial media

## 🛠 Teknologi yang Digunakan

- **HTML** untuk struktur dasar website
- **CSS** untuk styling dan responsivitas
- **JavaScript** untuk fungsionalitas dark mode dan interaktivitas
- **LocalStorage API** untuk menyimpan preferensi mode tampilan pengguna
- **Flexbox** dan **Grid** untuk layout yang responsif
- **Media Queries** untuk optimasi pada berbagai ukuran layar

## 📂 Struktur Direktori

```
├── index.html          Halaman utama website
├── about.html          Halaman tentang pemilik
├── portfolio.html      Halaman portfolio proyek
├── contact.html        Halaman kontak
├── style.css           File CSS untuk styling semua halaman
├── L200230210.jpg      Foto profil
```

## 💡 Implementasi Fitur Utama

### Dark Mode Toggle
Website menerapkan fitur dark mode yang memungkinkan pengguna untuk beralih antara tampilan terang dan gelap. Preferensi ini disimpan menggunakan localStorage sehingga tetap aktif saat pengguna kembali ke website.

```javascript
const darkModeToggle = document.getElementById('darkModeToggle');
const body = document.body;

const enableDarkMode = () => {
    body.classList.add('dark-mode');
    localStorage.setItem('darkMode', 'enabled');
};

const disableDarkMode = () => {
    body.classList.remove('dark-mode');
    localStorage.setItem('darkMode', 'disabled');
};
```

### Responsive Design
Website dirancang dengan pendekatan responsive menggunakan CSS modern:

```css
.proyek-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}

@media (max-width: 600px) {
    .social-link {
        padding: 12px 25px;
        font-size: 1em;
    }
}
```

### Interactive Elements
Elemen interaktif seperti tombol dan link memiliki efek hover untuk meningkatkan pengalaman pengguna:

```css
.social-link:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 10px rgba(0, 0, 0, 0.3);
    background-color: #0056b3;
}
```

