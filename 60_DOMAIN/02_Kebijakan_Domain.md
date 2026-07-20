# Kebijakan Domain

## Hubungan Konseptual

Posisi Kebijakan di dalam arsitektur pengetahuan Nalakara diatur oleh rantai hubungan berikut:

Realitas
  ↓
Domain memodelkan Realitas
  ↓
Kebijakan (*Policy*) menjaga koherensi Domain
  ↓
Platform mengevaluasi dan menegakkan Kebijakan
  ↓
Implementasi tetap setia terhadap Realitas melalui Kebijakan

---

## Hakikat Kebijakan (Essence)

Kebijakan adalah **deklarasi batasan semantik yang menetapkan kriteria keabsahan bagi transisi keadaan (*State*) dan pembentukan hubungan (*Relation*) di dalam batas Domain.**

Secara ontologis, Kebijakan berkedudukan sebagai deklarasi pasif yang melekat pada model konseptual Domain. Kebijakan tidak melakukan tindakan, tidak memproses komputasi, dan tidak mengevaluasi dirinya sendiri.

---

## Sifat Inheren Kebijakan (Property)

Setiap Kebijakan wajib memiliki sifat-sifat bawaan berikut agar sah diakui oleh Platform:

### 1. Tercatat Secara Historis (Versioned Knowledge)
Kebijakan bersifat tetap untuk setiap versi yang telah dibekukan. Kebijakan dapat berevolusi seiring perubahan pemahaman terhadap realitas, namun setiap perubahan melahirkan versi kebijakan baru tanpa memodifikasi sejarah versi sebelumnya.

### 2. Deklaratif Murni
Kebijakan hanya menetapkan kondisi batas keabsahan (*what*), bukan prosedur evaluasi atau langkah pemeriksaan (*how*).

### 3. Deterministik
Evaluasi terhadap kondisi yang sama berdasarkan versi kebijakan yang sama wajib selalu menghasilkan keputusan keabsahan yang identik.

### 4. Bebas Kontradiksi
Kebijakan dilarang saling bertentangan secara logis dengan kebijakan lain di dalam domain yang sama pada versi kebijakan yang sama.

### 5. Dapat Diverifikasi (Verifiable)
Setiap kebijakan harus memiliki kriteria pembuktian yang objektif sehingga dapat ditentukan secara biner (Valid atau Tidak Valid) apakah suatu keadaan memenuhinya atau tidak. Jika suatu pernyataan tidak dapat diverifikasi secara objektif, pernyataan tersebut tidak sah sebagai Kebijakan.

---

## Batas Otoritas (Consequence)

Konsekuensi logis dari hakikat pasif Kebijakan diatur oleh batas-batasan berikut:

### 1. Pemisahan Peran
Domain bertanggung jawab mendeklarasikan Kebijakan secara pasif, sedangkan Platform bertanggung jawab mengevaluasi dan menegakkan Kebijakan tersebut secara aktif.

### 2. Batas Otoritas Semantik
Kebijakan suatu Domain hanya mengikat elemen Metamodel yang berada di dalam batas semantiknya sendiri dan tidak berlaku untuk domain lain.

---

## Aturan Deklarasi Kebijakan (Aturan Normatif)

Penyusunan Kebijakan di tingkat Domain wajib mematuhi aturan normatif berikut:

### 1. Larangan Prosedural (Anti-Imperative)
Kebijakan ditulis sebagai pernyataan kondisi batas, bukan sebagai instruksi bersyarat (*if-else*) atau prosedur penanganan kesalahan.

### 2. Keterlacakan Elemen
Setiap deklarasi kebijakan wajib mengacu secara eksplisit pada elemen Metamodel (Entitas, Keadaan, Hubungan, atau Perubahan) yang diaturnya.

### 3. Kebebasan Teknis
Kebijakan dilarang terkontaminasi oleh istilah, batasan, atau format teknologi implementasi fisik.

---

## Di Luar Tanggung Jawab Kebijakan (Out of Scope)

* Prosedur, algoritma, atau kode program pengecekan aturan.
* Berkas konfigurasi sistem (seperti YAML atau JSON).
* Kode kesalahan (*error code*) dan penanganan eksepsi.
* Alur kerja (*workflow*) yang dikomposisikan oleh produk.
