# Taksonomi Kapabilitas

Dokumen ini menetapkan aturan normatif mengenai sistem klasifikasi dan tata bahasa pengelompokan Kapabilitas di dalam Layer 50. Dokumen ini mendefinisikan aturan dan kriteria klasifikasi yang harus dipatuhi ketika menyusun kategori kapabilitas pada masa depan.

---

## Definisi dan Tujuan Taksonomi

Taksonomi Kapabilitas adalah spesifikasi sistem klasifikasi resmi yang mengatur tata cara mengelompokkan Kapabilitas Nalakara Platform berdasarkan karakteristik Kapasitas Inheren (Disposisi) yang mereka miliki.

Tujuan Taksonomi ini adalah untuk:
- Menyediakan kerangka pengorganisasian yang konsisten bagi seluruh kapabilitas di dalam repositori;
- Mencegah tumpang tindih batas konseptual antar kelompok kapabilitas;
- Menjamin kepatuhan klasifikasi terhadap fondasi ontologis Metamodel;
- Mengatur evolusi struktur penyimpanan pengetahuan secara tertib seiring berkembangnya kemampuan platform.

---

## Prinsip Klasifikasi

Setiap pengelompokan Kapabilitas di dalam Layer 50 wajib mengikuti prinsip klasifikasi berikut:

### 1. Berdasarkan Orientasi Disposisi Metamodel
Klasifikasi dibentuk berdasarkan jenis perlakuan inheren (Disposisi) yang diberikan oleh kapabilitas terhadap elemen-elemen Metamodel, bukan berdasarkan kemiripan fungsionalitas teknologi atau alur kerja bisnis.

### 2. Ortogonalitas Antar-Kelompok
Setiap kategori yang dibentuk dalam taksonomi harus bersifat saling lepas secara konseptual. Tidak boleh ada kategori yang definisinya tumpang tindih atau menjadi sub-bagian dari definisi kategori lainnya.

### 3. Kejelasan Batas Kategori
Setiap kategori wajib memiliki batas ruang lingkup yang didefinisikan secara tegas melalui kriteria inklusi (apa yang masuk) dan kriteria eksklusi (apa yang keluar) yang objektif.

---

## Aturan Penempatan Kapabilitas

Penempatan Kapabilitas individual ke dalam struktur taksonomi diatur oleh ketentuan berikut:

* **Penempatan Tunggal (Monotaksonomi)**: Setiap kapabilitas wajib ditempatkan di bawah satu dan hanya satu kategori taksonomi. Penempatan ganda dilarang.
* **Dominasi Disposisi**: Jika suatu kapabilitas menunjukkan karakteristik yang melintasi beberapa kategori, penempatan ditentukan berdasarkan jenis disposisi yang paling dominan dan esensial bagi identitas kapabilitas tersebut.
* **Kemandirian Relasional**: Penempatan suatu kapabilitas tidak boleh dipengaruhi oleh ketergantungan relasionalnya dengan kapabilitas lain, melainkan murni berdasarkan hakikat disposisinya sendiri.

---

## Aturan Struktur dan Hierarki

* **Kesederhanaan Hierarki**: Struktur taksonomi harus dijaga agar tetap sedatar (*flat*) mungkin. Penggunaan sub-kategori (hierarki bertingkat) hanya diizinkan apabila terbukti secara konseptual meningkatkan kejelasan batas ruang lingkup tanpa menambah kompleksitas administratif.
* **Ketertiban Kodifikasi**: Setiap kapabilitas yang berhasil ditempatkan wajib diberi kode penomoran yang mencerminkan kategori induknya dalam struktur penyimpanan file repositori.

---

## Aturan Evolusi Taksonomi

Evolusi terhadap struktur taksonomi (penambahan, modifikasi, atau penghapusan kategori) diatur oleh hukum evolusi berikut:

* **Uji Ketiadaan Wadah Semantik**: Kategori baru hanya boleh ditambahkan jika terdapat usulan Kapabilitas sah yang terbukti tidak dapat dipetakan secara logis ke dalam kategori-kategori yang sudah ada tanpa merusak batas semantik kategori tersebut.
* **Konsistensi Retrospektif**: Penambahan atau perubahan kategori tidak boleh merusak keterlacakan konseptual kapabilitas yang sudah ada ke lapisan fondasi. Setiap perubahan struktur wajib disertai dengan penyelarasan ulang terhadap seluruh kapabilitas yang terpengaruh.
