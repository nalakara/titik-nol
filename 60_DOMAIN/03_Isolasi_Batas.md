# Isolasi Batas

## Hubungan Batas dengan Realitas

Realitas bersifat tak terbatas dan saling terhubung tanpa sekat konseptual.

Batas (*Boundary*) berfungsi sebagai alat konseptual untuk mengisolasi satu aspek spesifik dari realitas agar dapat dimodelkan oleh Domain secara terfokus. Batas bukan pemisah fisik realitas, melainkan perimeter yang membatasi ruang pemahaman manusia terhadap realitas yang sedang dimodelkan.

---

## Hakikat Batas (Essence)

Batas adalah **perimeter logis yang membatasi ruang lingkup kepemilikan dan interpretasi makna dari seluruh konsep di dalam suatu Domain.**

Secara ontologis, Batas merupakan konsekuensi dari identitas Domain. Batas ada secara dinamis untuk melindungi integritas makna di dalam Domain sepanjang evolusi pemodelan terhadap realitas.

---

## Sifat Inheren Batas (Property)

Setiap Batas memiliki sifat bawaan berikut yang menjaga kestabilan konseptual Domain:

### 1. Kemandirian Semantik
Makna setiap konsep di dalam Batas tidak dapat dipengaruhi, diintervensi, atau diubah oleh konsep lain dari luar Batas.

### 2. Kesatuan Makna
Seluruh elemen di dalam Batas wajib merujuk pada satu interpretasi makna yang seragam dan konsisten.

---

## Konsekuensi Logis (Consequence)

Berdasarkan hakikat dan sifat inheren yang dimilikinya, keberadaan Batas melahirkan konsekuensi konseptual berikut:

### 1. Yurisdiksi Kebijakan
Kebijakan yang dideklarasikan oleh Domain secara logis hanya memiliki daya ikat dan berlaku di dalam Batas Domainnya sendiri.

### 2. Komposabilitas Lintas Batas
Karena Batas memutus ketergantungan langsung antar-domain, setiap interaksi lintas-batas menuntut adanya lapisan khusus di luar Domain (seperti Layer Produk) untuk merangkai perilaku secara komposit.

---

## Aturan Isolasi Batas (Aturan Normatif)

Perancangan dan pemeliharaan Batas wajib mematuhi aturan normatif berikut:

### 1. Hukum Ketergantungan Nol (Zero Coupling)
Dokumen Domain dilarang merujuk, mengimpor, atau bergantung secara langsung pada konsep yang didefinisikan oleh Domain lain.

### 2. Kemandirian Representasi Konseptual
Apabila dua Domain memodelkan aspek realitas yang tampak serupa, masing-masing Domain harus mendefinisikannya secara mandiri sesuai kesatuan maknanya sendiri, tanpa berbagi definisi konseptual secara langsung.

### 3. Larangan Intervensi Semantik
Definisi makna, transisi keadaan, dan hubungan internal di dalam suatu Domain dilarang diintervensi atau dipengaruhi secara langsung oleh Domain lain.

---

## Di Luar Tanggung Jawab Batas (Out of Scope)

* Dinding api (*firewall*) atau lingkungan isolasi komputasi (*sandbox*) teknis.
* Struktur pengelompokan kode program (seperti namespace atau package).
* Pemisahan fisik database atau infrastruktur penyimpanan data.
* Mekanisme otorisasi keamanan atau daftar kontrol akses (*ACL*).
