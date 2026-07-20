# Kapabilitas Otorisasi

Kapabilitas Otorisasi adalah kemampuan inheren Nalakara Platform untuk mengevaluasi dan memutuskan apakah suatu Aktor atau Entitas diperkenankan melakukan suatu tindakan operasional terhadap Entitas, Keadaan, Hubungan, atau ruang konseptual tertentu berdasarkan hukum-hukum konseptual yang berlaku pada Platform.

---

## Tujuan

Kapabilitas ini diperlukan untuk menjamin ketertiban perilaku sistem dan menegakkan tanggung jawab aksi di dalam platform. Hal ini memastikan bahwa tidak ada perubahan keadaan, penembusan batas, atau manipulasi hubungan yang dapat dieksekusi secara ilegal tanpa adanya kelayakan hak aksi yang sah dari aktor yang memicunya.

---

## Disposisi Inheren

Melalui Kapabilitas Otorisasi, platform memiliki kapasitas bawaan untuk:
- **Evaluasi Kelayakan Tindakan**: Menilai apakah suatu tindakan yang diusulkan oleh suatu Entitas (Aktor) terhadap objek tertentu mematuhi hak kelayakan aksi yang telah ditetapkan.
- **Pemberian atau Penolakan Izin**: Menetapkan keputusan formal secara biner (Diperbolehkan atau Ditolak) terhadap suatu rencana aksi sebelum aksi tersebut diaktualisasikan menjadi perilaku sistem.
- **Peta Kewenangan Konseptual**: Menghubungkan tipe Entitas aktif (Aktor) dengan batas-batas ruang keadaan dan jenis hubungan yang diizinkan untuk diakses atau diubah olehnya.

---

## Invarian

Selama Kapabilitas Otorisasi berlaku, hukum-hukum berikut selalu benar dan tidak boleh dilanggar:
- **Kemandirian Keputusan**: Proses evaluasi otorisasi tidak boleh memodifikasi Keadaan, memutuskan Hubungan, mengubah Identitas, atau merusak Batas dari objek-objek yang sedang dievaluasi.
- **Konsistensi Keputusan**: Evaluasi otorisasi terhadap aktor, tindakan, objek, dan aturan yang sama pada koordinat waktu yang sama wajib menghasilkan keputusan (Izin atau Penolakan) yang identik.
- **Ketiadaan Otorisasi Implisit**: Tidak ada tindakan operasional lintas-batas atau perubahan keadaan yang dinyatakan sah di dalam platform tanpa melalui proses evaluasi otorisasi yang eksplisit.

---

## Batasan Kapabilitas

### Yang Termasuk Ruang Lingkup
- Penetapan aturan kewenangan konseptual yang memetakan hubungan kelayakan aksi antar-entitas.
- Evaluasi kelayakan aksi sebelum terjadinya transisi keadaan atau modifikasi hubungan.
- Penerbitan status keputusan otorisasi (Diizinkan / Ditolak) terhadap suatu rencana aksi.

### Yang Bukan Ruang Lingkup
- Pembuktian identitas aktor atau proses masuk sistem / login (tanggung jawab Kapabilitas Autentikasi yang berada di luar ruang lingkup dokumen ini).
- Pengamanan keunikan dan imutabilitas identitas Entitas (tanggung jawab Kapabilitas Pemeliharaan Identitas).
- Pengesahan transisi keadaan internal Entitas secara individual (tanggung jawab Kapabilitas Pengelolaan Perubahan).
- Pengelolaan batas-batas ruang konseptual (tanggung jawab Kapabilitas Pengelolaan Batas).
- Pengelolaan teknis mengenai Akun Pengguna (*User*), Peran (*Role*), Sesi (*Session*), Token Keamanan (*JWT*), atau integrasi penyedia identitas (*Identity Provider / IAM*) (tanggung jawab Layer Implementasi).

---

## Ketergantungan Ontologis

* **Prasyarat**: Kapabilitas ini secara mutlak bergantung pada Kapabilitas Pemeliharaan Identitas (`10_Identity_Preservation.md`), Kapabilitas Pengelolaan Keadaan (`20_State_Management.md`), Kapabilitas Pengelolaan Perubahan (`30_Change_Management.md`), Kapabilitas Pengelolaan Hubungan (`40_Relationship_Management.md`), Kapabilitas Keterlacakan (`50_Traceability.md`), Kapabilitas Validasi (`60_Validation.md`), dan Kapabilitas Pengelolaan Batas (`70_Boundary_Management.md`). Keputusan otorisasi tidak mungkin diambil tanpa adanya identitas aktor yang jelas, keadaan objek yang terpantau, rencana perubahan yang terdefinisi, hubungan relasional yang sah, rekam sejarah yang valid, kepatuhan semantik yang terverifikasi, dan batas-batas ruang yang ditegakkan.
* **Ketergantungan**: Kapabilitas ini menjadi landasan bagi penegakan aturan bisnis di Layer Domain Bisnis (`60_DOMAIN`) dan penentuan skema hak akses pada produk akhir.

---

## Implikasi Ketiadaan Kapabilitas

Without Kapabilitas Otorisasi, platform akan mengalami kegagalan sistematis sebagai berikut:
- **Anarki Tindakan**: Setiap entitas dapat memodifikasi keadaan objek lain secara sewenang-wenang melintasi batas-batas konseptual tanpa adanya kontrol kelayakan, yang merusak ketertiban sistem operasional.
- **Keruntuhan Akuntabilitas**: Platform kehilangan kemampuan untuk membuktikan kelayakan hak dari aktor yang memicu suatu peristiwa, sehingga integritas data tidak dapat dipertanggungjawabkan secara hukum konseptual.
- **Kebocoran Hak Akses Semantik**: Ketiadaan penegakan kewenangan konseptual akan melarutkan fungsi batas ruang semantik, yang membiarkan interaksi ilegal merusak struktur pengetahuan sistem.
