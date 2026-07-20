# Layer 60 — Domain

## Tujuan Layer

Layer Domain menyediakan pemodelan terstruktur atas aspek realitas tertentu dengan memberikan makna konseptual terhadap elemen-elemen Metamodel. Layer ini merumuskan hukum operasional realitas menjadi deklarasi konseptual yang bebas dari ketergantungan teknologi.

---

## Definisi Domain

Domain adalah **model konseptual yang merepresentasikan satu aspek realitas secara koheren.**

Setiap domain membatasi wilayah pengetahuannya sendiri secara semantik untuk menjaga kejelasan makna. Model konseptual ini dibangun dengan menggunakan elemen-elemen Metamodel dan memanfaatkan Kapabilitas Platform untuk memperlakukan elemen-elemen tersebut secara konsisten.

---

## Posisi dalam Arsitektur Pengetahuan

Layer Domain berada di bawah Layer Kapabilitas dan di atas Layer Produk.

```text
Kapabilitas
     ↓
  Domain
     ↓
  Produk
```

Domain memanfaatkan dan memberikan konteks terhadap kemampuan yang disediakan oleh Layer Kapabilitas, serta menyajikan model konseptual murni yang siap dirangkai menjadi alur kerja fungsional di Layer Produk.

---

## Hubungan Antar Layer

* **Hubungan dengan Layer Kapabilitas di Atasnya**:
  Domain bersifat pasif dan hanya mendeklarasikan Kebijakan (*Policy*) yang mengikat model konseptualnya. Kapabilitas Platform bertugas memelihara, mengevaluasi, dan menegakkan kebijakan tersebut agar integritas sistem tetap terjaga.
* **Hubungan dengan Layer Produk di Bawahnya**:
  Domain terisolasi secara mutlak dan tidak mengetahui keberadaan domain lainnya. Layer Produk bertindak sebagai kompositor yang merangkai perilaku (*Behavior*) dari berbagai domain terisolasi menjadi alur kerja lintas-domain (*workflows*) untuk disajikan sebagai solusi akhir bagi pengguna.

---

## Prinsip Layer Domain

1. **Pemodelan Realitas**: Domain memodelkan realitas yang sudah ada, bukan menciptakan realitas baru berdasarkan kenyamanan desain sistem atau keterbatasan perangkat lunak.
2. **Kemandirian Semantik**: Setiap domain memiliki otoritas penuh atas makna elemen pengetahuan di dalam batasnya. Makna suatu konsep tidak boleh dipengaruhi atau didefinisikan oleh domain lain.
3. **Deklarasi Pasif**: Domain hanya bertugas mengodifikasikan struktur pengetahuan dan kebijakan, sedangkan eksekusi operasional dan evaluasi aturan merupakan tanggung jawab platform.

---

## Ruang Lingkup

* Pemodelan tipe Entitas, Keadaan, Hubungan, dan Perubahan yang sah di dalam satu aspek realitas spesifik dengan menggunakan elemen-elemen Metamodel.
* Deklarasi Kebijakan (*Policy*) konseptual yang mengikat transisi keadaan dan hubungan entitas di dalam domain.
* Penegasan batas semantik yang memisahkan wilayah pengetahuan domain dari wilayah lainnya.

---

## Di Luar Tanggung Jawab Domain

* Pilihan database, teknologi, bahasa pemrograman, atau kerangka kerja (tanggung jawab Layer Implementasi).
* Desain antarmuka pengguna (UI/UX) dan penyusunan fitur produk akhir (tanggung jawab Layer Produk).
* Penyediaan mesin penegak aturan, penelusuran sejarah, atau manajemen data fisik (tanggung jawab Layer Kapabilitas).

---

## Daftar Dokumen Awal

Untuk memandu perancangan domain secara konsisten, layer ini diawali oleh dokumen-dokumen normatif berikut yang dapat dikembangkan lebih lanjut sesuai kebutuhan evolusi repositori:

* **[01_Domain.md](01_Domain.md)**: Menetapkan definisi, batasan ontologis, dan karakteristik dasar dari Domain di dalam Nalakara Platform.
* **[02_Kebijakan_Domain.md](02_Kebijakan_Domain.md)**: Mengatur tata cara dan aturan bagaimana domain mendeklarasikan Kebijakan (*Policy*) secara pasif agar kompatibel dengan platform.
* **[03_Isolasi_Batas.md](03_Isolasi_Batas.md)**: Menetapkan standar pembatasan semantik dan hukum larangan ketergantungan antar-domain (*zero coupling*).

---
Status          : Stable
Versi           : 1.0
Bahasa Asli     : Bahasa Indonesia
Dokumen Induk   : Peta Arsitektur Pengetahuan
