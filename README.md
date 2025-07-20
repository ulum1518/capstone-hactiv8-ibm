# 📊 Klasifikasi dan Ringkasan Berita Online dengan Bantuan AI

Proyek ini merupakan bagian dari Capstone Project Analisis Data menggunakan AI. Tujuannya adalah untuk membantu masyarakat memahami berita online secara cepat dan mudah melalui klasifikasi otomatis dan ringkasan yang sederhana.

---

## 📌 Latar Belakang

Banyak berita online di Indonesia ditulis dalam bentuk panjang dan kompleks, sehingga sulit dipahami oleh masyarakat umum, terutama peserta didik. Informasi penting seperti daftar temuan atau pelanggaran sering tersembunyi di tengah teks yang panjang. Proyek ini bertujuan untuk menyederhanakan isi berita dan mengekstrak poin-poin penting menggunakan model AI, sehingga pembaca bisa langsung memahami inti beritanya.

---

## 🎯 Tujuan Proyek

- Menyederhanakan konten berita agar mudah dipahami semua kalangan.
- Mengklasifikasikan elemen penting dari berita seperti kategori, tokoh, lokasi, isu, dan sentimen.
- Menghasilkan ringkasan otomatis yang mencakup poin utama dari berita.

---

## 🛠️ Tools & Teknologi

- 🧠 **LLM:** [Granite 3.3-8B Instruct (IBM) via Replicate](https://replicate.com/ibm-granite/granite-3.3-8b-instruct)
- 🔧 **Framework:** [LangChain](https://www.langchain.com/)
- 🌐 **Web Scraping:** `requests`, `BeautifulSoup4`
- 💻 **Platform:** Google Colab / Python

---

## ⚙️ Langkah-langkah Analisis

1. **Pengambilan Data:**  
   Scraping berita dari situs [detik.com](https://www.detik.com/](https://www.detik.com/edu/sekolah/d-7959673/4-temuan-kemendikdasmen-di-spmb-2025-jual-beli-kursi-pemalsuan-dokumen) menggunakan BeautifulSoup dan requests.
2. **Preprocessing:**  
   Membersihkan teks dari tag HTML, merapikan spasi, dan menyatukan paragraf.
3. **Prompt Engineering:**  
   Menyusun prompt terstruktur agar AI dapat mengklasifikasikan dan meringkas isi berita secara akurat.
4. **Analisis AI:**  
   Menggunakan model Granite 3.3-8B untuk menghasilkan klasifikasi dan ringkasan.
5. **Hasil & Evaluasi:**  
   Mengecek apakah output sudah mencakup poin penting seperti daftar temuan atau isu utama.

---

## 📈 Contoh Hasil (SPMB 2025)

**Klasifikasi berita**

*Kategori Utama*: Politik (karena terkait dengan instansi pemerintah dan proses pemilihan)

*Tokoh Utama*: Kemendikbud, SPMB (Badan Pemilihan Bantuan dan Pendidikan)

*Lokasi Kejadian*: Netral (tidak menyebutkan lokasi spesifik)

*Waktu Kejadian*: 20 Juli 2025 (walaupun tidak jelas apakah ini waktu publikasi berita atau waktu kejadian)

*Sentimen berita*: Negatif (karena berita mengungkap kasus pemalsuan dokumen)

*Isu Khusus*: Korupsi, keberlanjutan proses pemilihan

*Keaslian berita*: Fakta (tidak ada alasan menunjukkan hoaks)


**Ringkasan**

Kemendikbud, badan pemerintah yang bertanggung jawab untuk pendidikan, terdakwa melakukan pemalsuan dokumen selama proses pemilihan SPMB 2025. Berita menyebutkan empat (4) temuan yang menunjukkan kasus pemalsuan, salah identitas, dan penipuan. Ini menciptakan sentimen negatif karena menunjukkan potensi korupsi dalam proses pemilihan dan menyebabkan kebimbangan tentang keberlanjutan proses tersebut. Berita juga menyebutkan beberapa poin utama, seperti nama-nama individu yang terlibat dan tindakan yang diambil oleh Kemendikbud setelah penemuan tersebut.

---

## 🔍 Insight & Rekomendasi

### Insight:
- Terdapat praktik kecurangan serius dalam seleksi penerimaan peserta didik.
- Sistem seleksi belum sepenuhnya transparan dan aman dari penyalahgunaan.

### Rekomendasi:
- Terapkan verifikasi dokumen digital.
- Sediakan saluran pelaporan yang mudah dan aman.
- Audit sistem seleksi secara berkala di lembaga pendidikan.

---

## 🧠 Pembelajaran

- Teknik prompting yang spesifik dan terarah menghasilkan output AI yang lebih akurat.
- Peran manusia tetap penting untuk memeriksa dan memvalidasi hasil analisis AI.
- AI sangat membantu dalam mempercepat proses pemahaman informasi yang kompleks.

---
