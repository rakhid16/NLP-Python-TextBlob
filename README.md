# Pengantar Pengolahan Bahasa Alami dengan Python menggunakan TextBlob

<p align="center">
<img src="https://memegenerator.net/img/instances/72705299/come-and-do-nlp-join-the-dark-side.jpg" height="350"/></p>

<h3>Wajib Ngarti</h3>
<p>Pengolahan/Pemrosesan Bahsa Alami<i>(yang biasa disebut dengan Natural Language Processing)</i> merupakan cabang dari Kecerdasan Buatan yang mengombinasikan ilmu linguistik dan ilmu komputer. Tujuan dari pengolahan bahasa alami adalah melakukan pemodelan komputasi dari bahasa, sehingga dapat terjadi interaksi antara manusia dan mesin dengan perantara bahasa alami.</p>

<p>Setidaknya ada tujuh pembahasan dalam pengolahan bahasa alami, yakni:<br>
<b>1. Fonologi</b><br>Berhubungan dengan suara yang menghasilkan kata yang dapat dikenali. Bidang ini dipakai dalam aplikasi-aplikasi <i>speech based system</i><br>
<b>2. Morfologi</b><br>Pengetahuan tentang kata dan bentuknya sehingga bisa dibedakan antara yang satu dengan yang lain.<br>Contoh : Menyalahkan <br>prefiks : me-<br>kata dasar : salah<br><i>sufiks : -kan</i><br>
<b>3. Sintaksis</b><br>Pengetahuan tentang urutan kata dalam pembentukan kalimat.<br>Contoh :<br>Kalimat terdiri atas subjek lalu predikat<br>Subjek terdiri atas determinan lalu kata benda<br>Predikat terdiri atas kata kerja lalu kata benda<br>
<b>4. Semantik</b><br>Memelajari gabungan dari kata yang membentuk arti baru dari suatu kalimat yang utuh.<br>contohnya : Rakhman Wahid mahasiswa yang ringan tangan<i>(iya dong)</i>.<br>
<b>5. Pragmatik</b><br>pengetahuan tentang konteks kata/kalimat yang berhubungan erat dengan siatuasi pemakaian kalimat tersebut.<br>Contohnya : <br>Rakhman suka makan nasi goreng<br>Rakhman suka makan nasi goreng!<br>Rakhman suka makan nasi goreng?<br>
<b>6. <i>Discourse Knowledge</i></b><br>Pengetahuan tentang hubungan antar kalimat. Melakukan pengenalan apakah suatu kalimat yang telah dikenali mempengaruhi kalimat selanjutnya.<br>Contoh :<br>Rakhman membeli bakso di kantin. Ia tidak suka makan di sana<br>Kata "Ia" pada kalimat ke dua merujuk pada "Rakhman" di kalimat pertama dan kata "di sana" pada kalimat ke dua merujuk pada tempat "kantin" di kalimat pertama.<br>
<b>7. <i>Word Knowledge</i></b><br>Mencakup arti sebuah kata secara umum dan apakah ada arti khusus bagi kata tersebut dalam percakapan dengan konteks tertentu<i>(jelas paham'kan? heheheh)</i></p>

<p>Penerapan pengolahan bahasa alami terbagi menjadi dua, yakni <i>text-based application</i> dan <i>speech-based application</i>. Di mana <i>text-based application</i> diterapkan pada pemrosesan terhadap teks tulis. Contohnya mencari topik dalam berita, buku, email, menterjemahkan dokumen dll. Paham'kan? Pahamlah (: Sedangkan <i>speech-based application</i> aplikasi yang melakukan pemrosesan dari bahasa lisan atau pengenalan suara. Contohnya sistem pelayanan otomatis melalui telepon, kontrol suara pada peralatan elektronik, "Oke Google" dari Google Assistant dll. Pengolahan bahasa alami juga diterapkan dalam google terjemah, chatbot, analisis sentimen.</p>

<p align="center">
<img src="http://i1.kym-cdn.com/photos/images/newsfeed/000/531/557/a88.jpg" width="350"/></p>

<p align="center">Gramatika</p>
<p>Suatu aturan yang menentukan apakah suatu kumpulan kata dapat diterima sebagai kalimat oleh bahasa tersebut. Grammar dari Chomsky Hierarchy yaitu Context Free Grammar memiliki sifat lebih mudah dipahami perilakunya dan pengolahannya serta masih dapat diolah dalam bentuk yang terstruktur. CFG merepresentasikan bahwa suatu gramar itu dapat dibentuk dari empat elemen, yaitu : simbol awal, aturan penulisan, simbol non terminal, simbol terminal. Berikut contohnya</p>
<p align="center">
<img src="http://lh3.googleusercontent.com/RjxHtQAPOSuiAYvPQ7MGBjH9u4t5Xe2Hqh0-I_32Ok1TCcUA4i8BBSqEpLFQ0UzpBQkqEf0iO-Fr5oU-6j3aM_J3Z90qyZTd9eXuRD1keGxMNOQogwl_8CGHBZrvrcHHQUQJv_datlsntrkoO_MD-wpwK0HSzESF4hQIPAFjb3iWIw2xaBYOwqrnAn0rAi4Hu_8J3aLNa7Xv_hxR0Uj0xnLm7JqqbmAp3pQKUsE9IOlu9Lz1FxmAy7qgQYVYGmuSYbJreX4_-sHQRXz-PM5yg0ysCHIR28nEoUeweGgwkv1OR-ZfObk26EdZ1LMm5eqLK_GE5d2VKnbh23F7rXUh5tsANUqUzouwxd1DZjwhYQZQcvCc37orBcfwLplo_PHqErQhhYgAG71GNX71UMuBnB_BX01nq5sms2jwd-HAlTry26I-kkbBrw7B_lFCihIwHKF1bVKXqp2PRZ5SaW4Kpq1WbQM1uVf3I9X-lApzP5pGvP9YdnYd12AA0UnQA9fF9P0P-3X8WMdQeXH_3dCOhAWUCfdIPPqgZiYNuKCUDW31jNsCMBruSIACEM92wzvn00i4p5G8x4lrgrm6xZFnD2PL-muzUl04tBQw5Qd8Pr5pPxwn3yX9asUSOjMDL2Y6r50_0_HPRlPAw4TZgPnAAeeXGyuxkZ3P" width="350"/>
</p>

<p align="center">Parsing</p>
<p>Proses menganalisa suatu kumpulan kata dengan memisahkan kata-kata itu dan menentukan struktur sintaks dari tiap kata tersebut. Parsing dapat dibedakan menjadi dua yaitu Top-down parsing dan Bottom-up parsing. Berikut contohnya</p>
<p align="center">
<img src="http://lh3.googleusercontent.com/0LYPmnuvfKPTm56zVA0De2Jmq8Ra3Aa5Q6hx_9_Lul3wg634VI8978H8IeEMn-5S9vyC1qoU_Qd-lbS7BiMh-OyaX8m4GYh9TP5MViLnosd5wF5BVg54_LKeAbxPjCWwLN5bQpfTWRIjUNcEkhH70C_eTjQE_2Tf9oEpmizT88DSUEkJdgZxHc6KIXlibOLnpkgGHSfj21qw7Ikk1TGStdBAj_7kmcfcTSojHLTxqmVz6N2LmlzIPuNZki576VEfN2MYlWxE4WS0Li6Xb3TuB2rkmE55GPYpwoVwe1-luV9SAhFbhr7X1DkjqyB7uERwpt-N-oLcSQIQOB3SQmQQ-01419PQm-_5eCeiIqfMR9NzF0TNiW-DYVAZlC0YPAo0uZMnDQMs6ifcJw5Aw6fou3Jl82bbT-PW3cEwG_l4M6MBrIT0EFv_hyTetTcfF8wMyPIRmsNMDRP58L4_RSLpjVqgERxZf16e3ZTGRvVxamqeP-pYU45KhNA7INBj9oturtoY_9ald4kMNvZ945Z6eSLbA0dZ9jdoM9SOqGAzD1pkV6kZIbhNQWvdcS1LmQFtKFceVdRJWfdIjVMHfr1JAJBCjeIEi3b-w_lHzYeN94z7L2QIk_C1AVTncFpsWemUYolzCQ4eeC4AZztgFxKuXEfUdZp2DS-p" height="200" width="350" /><br>Kalau Top-down parsing pahamlah :v</p>

<p align="center">
<img src="https://memegenerator.net/img/instances/55005542/thats-all-i-have-to-say-about-that.jpg" /></p>
<h3>Peralatan</h3>
<p align="center">
<img src="https://www.python.org/static/img/python-logo.png" /></p>
<p>Saya saran'kan menggunakan Python vers 3 ke atas. Kenapa? Karena dukungan untuk python versi 2.7 sebentar lagi dihentikan dan untuk tutorial yang saya sediakan di sini menggunakan python versi 3 lebih tepatnya 3.6.2. Bagi pengguna Mac & Ubuntu kalian bisa ngoding langsung di terminal. Kalo pengguna windows kalian kudu unduh dulu .exe nya. Setelah itu install .exe nya kemudian install pip. Cari aja di Google "How to install pip in windows" gampang kok heheheh.</p>
  
<p align="center">
<img src="https://textblob.readthedocs.io/en/dev/_static/textblob-logo.png" width="300" height="350" /></p>
Karena tutorial pake NLTK sudah banyak dan TextBlob mudah digunakan untuk pemula jadi daya putuskan pake TextBlob aja heheheh. Cara installnya gampang. Kalo kalian berhasil install pip tinggal buka cmd(windows)/terminal (Mac & Ubuntu) terus ketik ini
<h5>pip install TextBlob</h5> atau <h5>pip install -U TextBlob</h5>terus enter
<h5>python -m textblob.download_corpora</h5>terus enter. Kalo proses unduh dan install'nya selesai kuy <a href="https://github.com/Rakhid16/NLP-Python-TextBlob/blob/master/Praktek.ipynb">PRAKTEK</a> (:
