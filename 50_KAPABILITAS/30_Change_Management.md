# Kapabilitas Pengelolaan Perubahan

Kapabilitas Pengelolaan Perubahan adalah kemampuan inheren Nalakara Platform untuk memperlakukan perubahan Keadaan sebagai peristiwa konseptual yang sah, konsisten, dan tetap menjaga integritas ontologis dari Entitas yang bersangkutan.

---

## Tujuan

Kapabilitas ini diperlukan untuk merepresentasikan dinamika transisi kondisi objek nyata ke dalam platform. Hal ini menjamin bahwa setiap perpindahan Keadaan tidak terjadi secara acak atau tidak sah, melainkan berjalan melalui hukum kausalitas konseptual yang memetakan Keadaan asal dan Keadaan tujuan secara presisi.

---

## Disposisi Inheren

Melalui Kapabilitas Pengelolaan Perubahan, platform memiliki kapasitas bawaan untuk:
- **Validasi Transisi Keadaan**: Menguji apakah perpindahan dari suatu Keadaan asal menuju Keadaan tujuan merupakan transisi yang diizinkan dalam ruang keadaan Entitas tersebut.
- **Pengikatan Peristiwa**: Menghubungkan setiap perubahan Keadaan secara langsung dengan pemicu perubahan (*pemicu peristiwa*) yang sah dalam realitas.
- **Konsistensi Transisi**: Menjamin bahwa selama proses perubahan berlangsung, integritas data dan hubungan Entitas tidak berada dalam kondisi yang bertentangan dengan Metamodel.

---

## Invarian

Selama Kapabilitas Pengelolaan Perubahan berlaku, hukum-hukum berikut selalu benar dan tidak boleh dilanggar:
- **Keabsahan Keadaan Asal dan Tujuan**: Setiap perubahan Keadaan wajib melibatkan Keadaan awal yang sah dan menghasilkan Keadaan akhir yang sah di dalam ruang keadaan Entitas.
- **Kekekalan Identitas**: Proses perubahan Keadaan tidak boleh memutuskan, memodifikasi, atau mengganti Identitas unik dari Entitas yang mengalami perubahan tersebut.
- **Keterikatan Eksistensial**: Perubahan Keadaan hanya dapat terjadi pada Entitas yang dideklarasikan ada dan memiliki Keadaan aktif yang sah saat proses perubahan dimulai.

---

## Batasan Kapabilitas

### Yang Termasuk Ruang Lingkup
- Validasi jalur transisi keadaan yang diizinkan untuk setiap tipe Entitas.
- Pengesahan peristiwa perubahan keadaan berdasarkan aturan konseptual platform.
- Penjaminan bahwa transisi keadaan berjalan secara utuh (tidak menyisakan keadaan menggantung/tidak valid).

### Yang Bukan Ruang Lingkup
- Pengamanan ketunggalan dan imutabilitas identitas Entitas (tanggung jawab Kapabilitas Pemeliharaan Identitas).
- Pemeliharaan keadaan aktif tunggal Entitas pada titik waktu tertentu (tanggung jawab Kapabilitas Pengelolaan Keadaan).
- Perekaman kronologi sejarah dan penelusuran asal-usul perubahan yang telah lalu (tanggung jawab Kapabilitas Keterlacakan).
- Pengelolaan antrean pesan (*message queue*), arsitektur *event-driven*, atau mekanisme basis data untuk menyimpan data perubahan (tanggung jawab Layer Implementasi).

---

## Ketergantungan Ontologis

* **Prasyarat**: Kapabilitas ini secara mutlak bergantung pada Kapabilitas Pemeliharaan Identitas (`10_Identity_Preservation.md`) and Kapabilitas Pengelolaan Keadaan (`20_State_Management.md`). Perubahan tidak dapat terjadi tanpa adanya Entitas dengan Identitas yang unik dan Keadaan aktif yang sah untuk diubah.
* **Ketergantungan**: Kapabilitas ini menjadi prasyarat logis bagi Kapabilitas Keterlacakan (*Traceability*) dan kapabilitas lainnya yang memerlukan pencatatan serta analisis terhadap jalannya transisi keadaan sistem.

---

## Implikasi Ketiadaan Kapabilitas

Tanpa Kapabilitas Pengelolaan Perubahan, platform akan mengalami kegagalan sistematis sebagai berikut:
- **Anarki Transisi**: Keadaan Entitas dapat melompat secara acak ke keadaan mana pun tanpa ada aturan validasi transisi, yang merusak keabsahan alur kerja operasional.
- **Kehilangan Kausalitas**: Platform tidak dapat menjelaskan mengapa atau bagaimana suatu Entitas berpindah dari satu Keadaan ke Keadaan lain, sehingga merusak pemodelan Realitas.
- **Kerusakan Keadaan Tengah (State Corruption)**: Kegagalan dalam menjamin penyelesaian perubahan dapat menyebabkan Entitas terperangkap dalam kondisi yang tidak konsisten atau tidak sah di dalam sistem.
