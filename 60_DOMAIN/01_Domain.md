# Domain

## Hubungan Domain dengan Realitas

Realitas hadir terlebih dahulu secara independen sebelum pemodelan dilakukan. Realitas merupakan sumber dari seluruh pengetahuan yang diamati dan dipahami oleh manusia.

Domain bertugas untuk mengamati dan merepresentasikan realitas tersebut secara konseptual. Domain tidak menciptakan realitas baru, tidak mengubah realitas yang ada, dan tidak memaksa realitas untuk menyesuaikan diri dengan representasi.

Domain bukanlah realitas itu sendiri. Domain adalah abstraksi pengetahuan mengenai aspek realitas tertentu yang disusun menggunakan tata bahasa Metamodel agar dapat dipahami dan dioperasionalkan secara konsisten.

---

## Hakikat Domain (Essence)

Domain adalah **model konseptual yang merepresentasikan satu aspek realitas secara koheren.**

Secara ontologis, Domain berkedudukan sebagai wadah pasif yang mengodifikasikan keteraturan semantik dari sekelompok konsep. Domain tidak memiliki kemampuan aktif untuk menjalankan perilakunya sendiri atau mengevaluasi aturannya secara mandiri.

Seluruh keputusan perancangan dan pemodelan Domain wajib tunduk sepenuhnya kepada realitas yang dimodelkan, bukan kepada kebutuhan implementasi fisik, batas teknologi, maupun kenyamanan perancangan perangkat lunak.

---

## Sifat Inheren (Property)

Setiap Domain memiliki sifat bawaan yang selalu melekat dan tidak dapat dipisahkan dari keberadaannya:

### 1. Koherensi Semantik
Seluruh konsep, entitas, keadaan, dan hubungan di dalam suatu Domain wajib memiliki keterikatan logis yang saling menerangkan. Kumpulan elemen tersebut harus membentuk satu kesatuan pemahaman yang utuh mengenai aspek realitas yang dimodelkan.

### 2. Keterikatan Batas Semantik
Setiap makna konsep, entitas, dan hubungan di dalam Domain terkunci secara mutlak di dalam batas semantiknya. Makna tersebut tidak berlaku, tidak dapat digunakan langsung, dan tidak boleh memengaruhi wilayah pengetahuan di luar batas domain tersebut.

### 3. Agnostisisme Fisik
Domain bersifat murni konseptual. Keberadaan dan definisi Domain tidak dipengaruhi oleh cara penyimpanan data, pemrosesan komputasi, bahasa pemrograman, kerangka kerja, atau pilihan teknologi implementasi fisik.

---

## Konsekuensi Logis (Consequence)

Berdasarkan hakikat dan sifat inheren yang dimilikinya, keberadaan sebuah Domain secara logis melahirkan efek-efek berikut:

### 1. Tegaknya Batas (Boundary)
Karena setiap Domain memiliki kemandirian semantik yang terisolasi, sekat pemisah (Batas) secara otomatis terbentuk secara logis untuk melindungi integritas makna di dalam domain tersebut dari pencampuran makna luar.

### 2. Kebutuhan Deklarasi Kebijakan (Policy)
Agar koherensi semantik di dalam domain tetap terjaga dari waktu ke waktu, Domain melahirkan kebutuhan untuk mendeklarasikan batasan semantik (Kebijakan) secara pasif, untuk kemudian dievaluasi dan ditegakkan oleh Kapabilitas Platform.

### 3. Isolasi Ketergantungan (Zero Coupling)
Sebagai konsekuensi dari kemandirian batas semantiknya, satu Domain secara logis tidak memiliki ketergantungan konseptual langsung terhadap Domain lainnya. Setiap interaksi lintas-domain diserahkan kepada koordinasi lapisan di luar Domain.

---

## Kriteria Kelayakan Domain

Penentuan pembentukan, pemisahan, dan penyatuan Domain diatur oleh ketentuan normatif berikut:

### 1. Kriteria Kelayakan sebagai Domain
Suatu aspek realitas layak dideklarasikan sebagai Domain mandiri jika ia memiliki sekelompok konsep yang saling bergantung untuk membentuk makna baru. Apabila aspek realitas tersebut dapat didefinisikan secara mandiri tanpa memerlukan struktur relasional dan transisi keadaan yang kompleks di dalamnya, ia cukup dimodelkan sebagai *Entitas* di bawah domain yang sudah ada.

### 2. Aturan Pemisahan Dua Domain
Dua domain wajib dipisahkan apabila terjadi pergeseran atau percabangan makna terhadap suatu objek yang sama (misalnya, ketika definisi objek tersebut memiliki logika states dan hubungan yang berbeda secara konseptual).

### 3. Aturan Penyatuan Dua Domain
Dua domain wajib disatukan apabila pemisahan keduanya menyebabkan hilangnya koherensi konseptual terhadap aspek realitas yang dimodelkan.
