# Dekomposisi Kapabilitas

Dokumen ini menetapkan aturan normatif untuk memisahkan, menggabungkan, memecah, dan mengelola evolusi Kapabilitas di dalam Layer 50. Seluruh penataan struktur dan taksonomi kapabilitas wajib mematuhi ketentuan di bawah ini.

---

## Dasar Pemisahan Kapabilitas

Pemisahan antara satu kapabilitas dengan kapabilitas lainnya didasarkan sepenuhnya pada keunikan Kapasitas Inheren (Disposisi) yang diberikan oleh platform untuk memperlakukan elemen Metamodel.

Pemisahan kapabilitas tidak boleh didasarkan pada elemen Metamodel yang dikelolanya secara eksklusif, melainkan pada esensi fungsi abstrak yang ditawarkan. Manifestasi perilaku (Behavior) yang muncul hanya digunakan sebagai bukti pendukung untuk mengenali eksistensi kapabilitas tersebut, bukan sebagai dasar klasifikasi utamanya.

---

## Penggabungan Kapabilitas

Dua kapabilitas wajib digabungkan menjadi satu jika memenuhi salah satu kondisi berikut:
- **Kesamaan Disposisi Inti**: Kedua kapabilitas bersumber dari kapasitas inheren yang sama pada platform, meskipun manifestasi perilakunya tampak berbeda secara visual atau operasional.
- **Keterikatan Konseptual Mutlak**: Salah satu kapabilitas kehilangan arti keberadaan atau tidak dapat didefinisikan secara utuh apabila kapabilitas lainnya dihilangkan dari sistem.

---

## Pemecahan Kapabilitas

Sebuah kapabilitas wajib dipecah menjadi dua atau lebih kapabilitas mandiri jika memenuhi salah satu kondisi berikut:
- **Multi-Disposisi**: Kapabilitas tersebut mengemban lebih dari satu kapasitas inheren platform yang secara konseptual tidak saling mengikat.
- **Kemandirian Evolusi Kapasitas**: Satu bagian dari kapasitas tersebut dapat diubah aturan inherennya tanpa mengganggu atau mengubah identitas konseptual kapasitas bagian lainnya.

---

## Ortogonalitas Kapabilitas

Dua kapabilitas dinyatakan ortogonal apabila masing-masing merepresentasikan kapasitas inheren yang berbeda dan dapat berevolusi secara independen tanpa mengubah identitas konseptual satu sama lain.

Kemiripan pada manifestasi perilaku (Behavior) yang muncul di permukaan tidak membatalkan ortogonalitas kedua kapabilitas, selama hakikat kapasitas inheren yang melahirkannya berbeda secara ontologis.

---

## Atomisitas Kapabilitas

Kapabilitas merupakan unit terkecil dari kapasitas platform. Pemecahan kapabilitas di bawah batas atomnya akan menghilangkan sifat disposisinya dan mengubahnya menjadi sekadar perilaku operasional (Behavior) atau tata cara teknis (Implementasi).

---

## Evaluasi dan Evolusi Kapabilitas

Setiap penambahan atau perubahan kapabilitas baru di dalam repositori harus dievaluasi secara ketat berdasarkan urutan keputusan berikut:

### 1. Evaluasi Kelayakan Ontologis
Memastikan usulan baru benar-benar merupakan kapasitas inheren platform (Disposisi), bukan merupakan aktualisasi tindakan (Behavior), alur bisnis (Domain), produk, atau detail teknis (Implementasi). Usulan yang gagal pada tahap ini wajib ditolak atau dipindahkan ke layer yang sesuai.

### 2. Evaluasi Kemandirian Konteks dan Teknologi
Memastikan usulan baru bersifat bebas konteks domain bisnis dan bebas dari ketergantungan teknologi tertentu.

### 3. Evaluasi Ortogonalitas
Memastikan usulan baru memiliki kapasitas inheren yang terpisah secara konseptual dari kapabilitas yang sudah ada dan dapat dikembangkan secara mandiri tanpa merusak identitas konseptual kapabilitas lainnya. Jika terdapat tumpang tindih disposisi, usulan baru harus digabungkan atau memperluas kapabilitas yang telah ada.
