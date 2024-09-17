Berikut adalah template `README.md` untuk proyek GitHub Anda terkait aplikasi **PuLID-FLUX** yang menggunakan Gradio:

---

# PuLID-FLUX: Pure and Lightning ID Customization via Contrastive Alignment

![PuLID-FLUX](https://i.ibb.co.com/ynqKvrr/banner-pulid.jpg)

PuLID-FLUX adalah aplikasi berbasis AI untuk menyesuaikan gambar wajah melalui **Contrastive Alignment**. Aplikasi ini dibangun menggunakan Gradio dan mendukung kustomisasi mendalam untuk menghasilkan gambar beresolusi tinggi. PuLID-FLUX memberikan kemampuan untuk mengubah detail gambar wajah dengan berbagai parameter yang dapat disesuaikan, seperti **timestep to start inserting ID**, **true CFG scale**, dan banyak lagi.

![Gradio](https://github.com/user-attachments/assets/bed5eb12-3592-4a48-ae25-92ebd061de8d)
[![Open in Spaces](https://huggingface.co/datasets/huggingface/badges/resolve/main/open-in-hf-spaces-xl-dark.svg)](https://deddy-pulid-flx-gpu.hf.space)

## Fitur Utama
- **Kustomisasi Wajah**: Sesuaikan gambar wajah dengan parameter mendetail untuk menghasilkan gambar berkualitas tinggi.
- **Dukungan Multi-Parameter**: Gunakan parameter seperti `prompt`, `guidance`, `true CFG scale`, `timestep to start`, dll.
- **Gradio Interface**: Antarmuka berbasis web yang mudah digunakan, dibangun menggunakan framework Gradio.
- **Integrasi API Gradio Client**: Memanfaatkan API Gradio untuk mengirim gambar dan menerima hasil kustomisasi gambar.
- **Latar Belakang Gradasi**: Antarmuka yang modern dengan latar belakang gradasi dan desain responsif.

## Instalasi

### Prasyarat
- Python 3.8 atau lebih baru
- [Pillow](https://python-pillow.org) untuk pengolahan gambar
- [Gradio](https://gradio.app) untuk antarmuka
- [Gradio Client](https://gradio.app/docs/#client) untuk menghubungkan API

### Langkah-langkah Instalasi

1. **Clone Repositori:**
   ```bash
   git clone https://github.com/username/PuLID-FLUX.git
   cd PuLID-FLUX
   ```

2. **Install dependensi:**
   Install semua dependensi yang diperlukan dari `requirements.txt` atau langsung:
   ```bash
   pip install gradio gradio_client Pillow numpy
   ```

3. **Jalankan Aplikasi:**
   Untuk menjalankan aplikasi:
   ```bash
   python app.py
   ```

## Penggunaan
Setelah aplikasi dijalankan, Anda dapat membuka antarmuka Gradio di browser. Ikuti langkah-langkah berikut:

1. **Masukkan Prompt:** Berikan deskripsi singkat tentang gambar yang ingin dihasilkan, misalnya "portrait, color, cinematic".
2. **Unggah Gambar Wajah:** Unggah gambar wajah yang ingin Anda kustomisasi.
3. **Sesuaikan Parameter:** Ubah parameter seperti `guidance`, `timestep to start`, `true CFG scale`, dll.
4. **Hasilkan Gambar:** Klik tombol `⭐ Mulai Generate Image ⭐`, dan hasil akan muncul dalam beberapa detik.

## Parameter Kustomisasi
- **Timestep to start inserting ID:** Nilai lebih kecil menghasilkan gambar yang lebih mirip dengan input ID, tetapi dengan fleksibilitas pengeditan yang lebih sedikit. Nilai yang lebih tinggi memberikan fleksibilitas pengeditan yang lebih besar tetapi dengan kemiripan yang lebih rendah.
- **True CFG Scale:** Dalam banyak skenario, disarankan untuk menggunakan skala true CFG sebesar 1 dan menyesuaikan guidance scale untuk efisiensi.

## Tips Penggunaan
- Untuk adegan fotorealistik, kami merekomendasikan menggunakan nilai `4` untuk `timestep to start inserting ID`.
- Untuk adegan bergaya, nilai `0-1` lebih sesuai.
- Jika Anda ingin mengetahui lebih lanjut tentang model dan pengaturannya, silakan lihat [Dokumentasi GitHub](https://github.com/ToTheBeginning/PuLID).

## CSS Kustom
Kami telah menerapkan **CSS kustom** untuk antarmuka Gradio, dengan latar belakang gradasi yang lembut dan warna font **silver** untuk pengalaman visual yang lebih menarik.

```css
#col-right {
    background: linear-gradient(180deg, #677D6A, #40534C);
    color: silver;
    padding: 10px;
    border-radius: 15px;
}
```

## Kontribusi
Kami menyambut kontribusi dari siapa pun. Jika Anda ingin berkontribusi:

1. Fork repositori ini.
2. Buat branch fitur baru (`git checkout -b fitur-anda`).
3. Lakukan commit perubahan (`git commit -m 'Tambah fitur XYZ'`).
4. Push ke branch (`git push origin fitur-anda`).
5. Buat Pull Request.

## Lisensi
Proyek ini dilisensikan di bawah lisensi MIT. Lihat [LICENSE](./LICENSE) untuk informasi lebih lanjut.

---

Semoga template ini membantu! Anda bisa menyesuaikan detail seperti URL gambar dan penjelasan sesuai kebutuhan proyek Anda.
