# Ketergantungan

Tidak ada sistem yang sepenuhnya berdiri sendiri. Setiap komponen dapat memerlukan pengetahuan, layanan, maupun kemampuan yang dimiliki oleh komponen lain. Dalam Nalakara, hubungan tersebut dipahami sebagai ketergantungan.

Ketergantungan memungkinkan komponen bekerja sama tanpa harus memiliki seluruh pengetahuan maupun tanggung jawab di dalam dirinya sendiri. Dengan membatasi ketergantungan pada hal-hal yang benar-benar diperlukan, setiap komponen dapat tetap fokus pada tanggung jawab utamanya sekaligus menjadi bagian dari sistem yang lebih besar.

Dalam Nalakara, ketergantungan harus dibangun secara sadar dan dapat dijelaskan berdasarkan kebutuhan pengetahuan, bukan semata-mata karena kemudahan implementasi. Sebuah komponen bergantung pada komponen lain karena membutuhkan kemampuan yang memang berada di luar ruang lingkup tanggung jawabnya, bukan karena batas arsitekturalnya tidak jelas.

Semakin jelas batas tanggung jawab setiap komponen, semakin sederhana pula ketergantungan yang terbentuk. Ketergantungan yang tepat memungkinkan perubahan dilakukan secara terarah tanpa menimbulkan dampak yang tidak perlu terhadap bagian lain dalam sistem. Sebaliknya, ketergantungan yang tidak terkendali dapat mengaburkan tanggung jawab, mengurangi kemandirian komponen, dan menyulitkan evolusi arsitektur.

Perubahan terhadap suatu komponen tidak selalu mengharuskan perubahan pada komponen yang bergantung kepadanya. Selama makna, tanggung jawab, dan bentuk interaksi tetap dipertahankan, setiap komponen dapat berkembang secara mandiri tanpa mengganggu konsistensi keseluruhan sistem.

Dengan demikian, ketergantungan bukan sekadar hubungan antar komponen, melainkan cara menjaga keseimbangan antara kerja sama, kemandirian, dan keberlanjutan arsitektur Nalakara.