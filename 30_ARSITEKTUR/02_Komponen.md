# Komponen

Setiap sistem dibangun dari berbagai bagian yang memiliki tanggung jawab masing-masing. Dalam Nalakara, setiap bagian tersebut disebut sebagai komponen.

Komponen merupakan representasi arsitektural dari satu tanggung jawab yang utuh. Sebuah komponen dibentuk untuk mengelola satu ruang lingkup pengetahuan secara konsisten tanpa mengambil tanggung jawab yang menjadi milik komponen lain. Dengan demikian, keseluruhan sistem dapat berkembang melalui kerja sama berbagai komponen yang memiliki peran yang jelas.

Keberadaan sebuah komponen tidak ditentukan oleh bentuk implementasinya. Sebuah komponen dapat diwujudkan sebagai modul, layanan, pustaka, proses, maupun bentuk teknis lainnya. Selama tanggung jawab yang diembannya tetap sama, perubahan implementasi tidak mengubah identitas arsitektural komponen tersebut.

Dalam Nalakara, setiap komponen memiliki batas tanggung jawab yang tegas. Komponen bertanggung jawab terhadap pengetahuan yang berada di dalam ruang lingkupnya, sementara hubungan dengan komponen lain dilakukan melalui interaksi yang jelas dan dapat dipahami. Dengan cara ini, perubahan pada satu komponen dapat dilakukan tanpa harus mengubah keseluruhan sistem.

Komponen tidak dirancang untuk berdiri sendiri, melainkan untuk bekerja bersama sebagai bagian dari satu arsitektur yang utuh. Kemandirian setiap komponen memungkinkan sistem berkembang secara bertahap, sedangkan keterhubungan antar komponen menjaga konsistensi perilaku seluruh ekosistem.

Dengan demikian, komponen bukan sekadar bagian dari perangkat lunak, melainkan satuan tanggung jawab arsitektural yang memungkinkan pengetahuan diwujudkan menjadi sistem yang modular, konsisten, dan berkelanjutan.