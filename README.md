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
<img src="https://lh3.googleusercontent.com/6LZKMcCKb_ObYjrxmhhv3dkC5sQo41Y99DUBr9K_FEyJyF2SHBfHwU3EfyPmLKw4tP4bu_EfmdAcTNWmmUiQlmR3lxUbnbWD7DFtbDfQJmG2CnWiAjgtSVjjRKGVBIACamBmsfjNrf5-ruxfLHxWw_kPbJQedM_uC1tWb6D9SfiIxCVefDbwyYPRb287pXbPAQK5_0YY_FwA3WaABhSlgz26Uym2czBm0Mu9o1PcWcSB_grFlMkqdt1nUazYOg6Pnl6dCSy5hquTFCUXKC3LJyisuHRFR3xCzBaWzn5A-pZuWDM2ywxo55s1My9-gmA72LnOm_CylTDz6wey_CZdP8Zt0g2NO9nwSq-BZcrhnvQgyUAu-J8bLxxUqOxDx-wPCadApvkvOlyDuSdsGPRoxN3jSeJY6exx3h53kHepvcoXEuF3EfALpxbXXoKEajwDawv22nIQzYhcfdMJL-8Aqw_vH2TuKJLmixPEFo_kEpCG2HBXBMTTUuVhpgoLd9tLKRWByDoSPKT6Ykj_ERfhC96Ga-9VFotAu3AyMomrarG3z304iI5L9jVbl4fsEZztXLpUfvE2xiYS85pC35uP0lCKw4Gib4u-pNtn2us=w870-h440-no" width="350"/>
</p>

<p align="center">Parsing</p>
<p>Proses menganalisa suatu kumpulan kata dengan memisahkan kata-kata itu dan menentukan struktur sintaks dari tiap kata tersebut. Parsing dapat dibedakan menjadi dua yaitu Top-down parsing dan Bottom-up parsing. Berikut contohnya</p>
<p align="center">
<img src="https://lh3.googleusercontent.com/1TAqNu18cZ3o98dG-qcdn0Gb355SODkaYaFmQuHQWEQWuxHFmGvo5Vo5pSyfb3sxAnmnHLMQrQbtr_owX6lGvLBXXr-xlnVyy0sYKNUIimPHqL6YjqqC7QVAKqVK-6gB8zeiTBCBV3kgvsHb4YJMruvrsoYRXB6UWb5gbSjQ2uqMKTJo_svKdGbBVabiWQf7ol1ijDboLP9hQUKh1rDLPR-EfEoJuZUaHiloSZxycpjIZRHH-Wrx4_8YwqoMxUv_Ab2ctQJ-gfQbPny-oJsRUdL8WztOZSBRkCZQsIxN8joEfKtU1prFqJ4G55m5HmVAp_pIp3xe07fMb_SGiXhX2wGgShaNovXUxoui6yd-y2wKNzNVQub8OHQ-1oFmWSpRmGXy_Dt1ogtY8y4dPz10K8jqHL2ZDFprGv3Q7mBqTZ8Nm2qrgoKtXzYzASEwTN1vbXubgmOZpLDv-aW01DYMxFDfKANT5Xqq-_ERCBRuaLRLAcoYv6n2--ryzx3lxK6wErOOlFfHunBNII1UfbQH_XhHkJoRC7wgWjaxWsCuQsYUlE_vZgSw2M2iM3aMplD6sKSFN9Qnv-IlBlkWixXuZLMijHN4ayNa8Fn_L8c=w715-h452-no" height="200" width="350" /><br>Kalau Top-down parsing pahamlah :v</p>

<p align="center">
<img src="https://memegenerator.net/img/instances/55005542/thats-all-i-have-to-say-about-that.jpg" /></p>
<h3>Peralatan</h3>
<p align="center">
<img src="https://www.python.org/static/img/python-logo.png" /></p>
<p>Saya saran'kan menggunakan Python vers 3 ke atas. Kenapa? Karena dukungan untuk python versi 2.7 sebentar lagi dihentikan dan untuk tutorial yang saya sediakan di sini menggunakan python versi 3 lebih tepatnya 3.6.2. Bagi pengguna Mac & Ubuntu kalian bisa ngoding langsung di terminal. Kalo pengguna windows kalian kudu unduh dulu .exe nya. Setelah itu install .exe nya kemudian install pip. Cari aja di Google "How to install pip in windows" gampang kok heheheh.</p>
  
<p align="center">
<img src="https://textblob.readthedocs.io/en/dev/_static/textblob-logo.png" width="350" height="350" /></p>
Karena tutorial pake NLTK sudah banyak dan TextBlob mudah digunakan untuk pemula jadi daya putuskan pake TextBlob aja heheheh. Cara installnya gampang. Kalo kalian berhasil install pip tinggal buka cmd(windows)/terminal (Mac & Ubuntu) terus ketik ini
<h5>pip install TextBlob</h5> atau <h5>pip install -U TextBlob</h5>terus enter
<h5>python -m textblob.download_corpora</h5>terus enter. Kalo proses unduh dan install'nya selesai berarti laptop kalian dah siap! :D 
