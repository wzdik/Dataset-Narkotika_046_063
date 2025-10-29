# ⚖️ Dataset Putusan Pengadilan Negeri Mojokerto – Kasus Narkotika (2020–2024)

## 📘 Deskripsi Umum
Dataset ini berisi **50 putusan resmi Pengadilan Negeri Mojokerto** yang berkaitan dengan perkara **pidana narkotika dan psikotropika**.  
Data disusun dalam format tabular berdasarkan dokumen asli dari **Direktori Putusan Mahkamah Agung Republik Indonesia** untuk keperluan **analisis Temu Kembali Informasi (TKI)** dan **pemrosesan teks hukum (Legal Text Mining)**.

Dataset ini digunakan untuk:
- 🔍 Membangun sistem pencarian putusan berbasis teks (*Information Retrieval System*)
- 🧠 Melatih model klasifikasi teks hukum
- 📊 Menganalisis pola hukuman, pasal, dan barang bukti
- ⚙️ Mengembangkan model ekstraksi entitas hukum (nama terdakwa, pasal, hukuman)

---

## 📂 Struktur Dataset
Dataset tersimpan dalam file:
> 🗂️ `Soal Uts-TKI_063_046.xlsx`

File ini terdiri dari 5 kolom utama:

| Kolom | Deskripsi |
|--------|------------|
| **No** | Nomor urut putusan |
| **No Putusan** | Nomor resmi perkara (misal: `510/Pid.Sus/2024/PN Mjk`) |
| **Lembaga Peradilan** | Nama pengadilan (seluruhnya PN Mojokerto) |
| **Barang Bukti** | Daftar barang bukti yang disita dari terdakwa |
| **Amar Putusan** | Ringkasan amar, termasuk pasal, lama hukuman, dan denda |

---

## ⚖️ Contoh Data
| No Putusan | Barang Bukti | Amar Putusan |
|-------------|---------------|---------------|
| 77/Pid.Sus/2024/PN Mjk | 34 paket sabu berbagai kode (A–Z); 1 timbangan digital; 1 HP Vivo hitam | Sugeng als Komar Bin Kasmadi – Pasal 114 ayat (2) UU 35/2009; 9 tahun; denda Rp1.000.000.000 subsider 3 bulan |
| 135/Pid.Sus/2024/PN Mjk | 20 paket sabu total 33,121 g; timbangan digital; HP Vivo | Yanto Prasetyo Bin Yateno – Pasal 114 ayat (2) UU 35/2009; 10 tahun; denda Rp1.000.000.000 subsider 6 bulan |
| 510/Pid.Sus/2024/PN Mjk | 10 paket sabu 4,71 g; HP Vivo; uang Rp500.000 | Muhammad Rudianto Bin Sapari – Pasal 114 ayat (1) UU 35/2009; 8 tahun; denda Rp1.000.000.000 subsider 3 bulan |
| 406/Pid.Sus/2024/PN Mjk | 1 paket ganja kering ±6,68 g; HP iPhone 11; motor Scoopy | Agus Salim Bin Turkan – Pasal 111 ayat (1) UU 35/2009; 6 tahun; denda Rp1.000.000.000 subsider 3 bulan |

---

## 🧾 Ringkasan Statistik
| Atribut | Nilai |
|----------|--------|
| Jumlah Putusan | **50** |
| Rentang Tahun | **2020–2024** |
| Lembaga | **Pengadilan Negeri Mojokerto** |
| Rata-rata Lama Hukuman | **±7,5 tahun** |
| Denda Umum | **Rp1.000.000.000,-** |
| Pasal Dominan | **Pasal 112(1)** dan **Pasal 114(1)** UU No.35/2009 |
| Barang Bukti Umum | Sabu, Bong, Timbangan Digital, HP Oppo/Vivo, Uang Tunai |
| Jenis Kelamin Terdakwa | Mayoritas **laki-laki (98%)** |
| Umur Umum Terdakwa | 25–45 tahun |

---

## 🧠 Tujuan Penggunaan Dataset
Dataset ini dikembangkan dalam konteks **Ujian Tengah Semester (UTS) Mata Kuliah Temu Kembali Informasi (TKI)**, dengan tujuan:
1. Menunjukkan pemahaman konsep *preprocessing*, *indexing*, dan *information retrieval*.
2. Menggunakan data hukum nyata sebagai bahan uji pencarian dokumen berbasis teks.
3. Melatih sistem pencarian (*IR system*) dengan pendekatan TF-IDF atau Cosine Similarity.
4. Membentuk *corpus hukum digital* untuk penelitian lanjutan di bidang *Legal Data Science*.

---

## 🧩 Tahapan Pengolahan Data
1. **Ekstraksi Dokumen:** Mengambil data putusan dari situs MA (format PDF).  
2. **Preprocessing:** Menghapus metadata, header, watermark, dan elemen non-teks.  
3. **Normalisasi Teks:** Mengubah ke huruf kecil, menghapus tanda baca dan stopword.  
4. **Pembuatan Indeks:** Menyimpan hasil ke `.xlsx` sebagai dataset final siap analisis.  

---

## 💡 Potensi Analisis & Penelitian
- 🔍 *Information Retrieval* berbasis TF-IDF / BM25 pada teks hukum Indonesia.  
- 📊 Analisis pola hukuman vs berat barang bukti.  
- 🧠 Model klasifikasi teks hukum berbasis BERT/IndoBERT.  
- 📈 Visualisasi tren pasal dan lama hukuman dengan Streamlit / Power BI.  

---

## 👨‍💻 Penyusun Dataset
| Nama | NIM | Keterangan |
|-------|-----|-------------|
| **Muhammad Syahrul Bachtiar** | **202210370311046** | Penyusun Dataset & Pengerjaan semua soal |
| **Andika Nur Islamy** | **202210370311063** | Penyusun Dataset & Pengerjaan semua soal |

📚 **Institusi:** Universitas Muhammadiyah Malang  
🧩 **Mata Kuliah:** Temu Kembali Informasi (TKI)  
🎓 **Dosen Pengampu:** Bapak Galih Wasis Wicaksono

---

## 📄 Lisensi
Dataset ini bersifat **terbuka untuk keperluan akademik**, dengan ketentuan:
> “Dataset ini merupakan hasil kompilasi 50 putusan Pengadilan Negeri Mojokerto (2020–2024) dari situs Direktori Putusan Mahkamah Agung RI. Disusun oleh Muhammad Syahrul Bachtiar dan Andika Nur Islamy (2025).”

---

## 🏁 Penutup
Proyek ini merupakan bentuk kontribusi terhadap digitalisasi data hukum Indonesia untuk mendukung pengembangan **AI Hukum dan Open Legal Data**.  
Dengan dataset ini, diharapkan peneliti, mahasiswa, dan praktisi dapat memahami **pola penegakan hukum, korelasi pasal, serta konteks sosial dalam peradilan pidana**.

> 💬 “Data hukum yang terbuka adalah langkah pertama menuju keadilan yang transparan.”  
> — *Muhammad Syahrul Bachtiar & Andika Nur Islamy, 2025* ⚖️
