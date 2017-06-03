# Belajar Python 3

![photo_2017-06-02_02-43-32](https://cloud.githubusercontent.com/assets/16227352/26697854/bb434b3e-473d-11e7-90d9-92f715c59a38.jpg)

Belajar Bahasa Pemrograman Python 3

Untuk info selanjutnya, https://t.me/migrasilinux

# Diskusi - Awas di Makan Python !

## Disclaimer:

Materi yang di sampaikan adalah ilmu yang di serap secara otodidak, maka dari itu kesalahan sangat mungkin terjadi. Mohon di koreksi jika dirasa kurang pas atau salah. Kritik dan saran terbuka lebar, asalkan tidak out of topic. Supaya diskusi berjalan baik dan kondusif, saya akan memberikan sedikit aturan, antara lain:

1. Dilarang mengejek, menghina, atau membuat perasaan member lain tidak enak saat member tersebut mengaku tidak paham. Ayo kita bantu dia, setidaknya sampai dia paham.
2. Dilarang meragukan diri sendiri dengan berkata: “itu terlalu sulit buat saya”, dsb. Karena, melupakan ‘dia’ lebih sulit dari bahasa pemrograman apapun!
3. Materi yang di sampaikan boleh di interupsi, di kritik, atau di benarkan jika dirasa kurang pas.
4. Penyampaian materi akan di sampaikan minimal satu sub-bab setiap harinya pada jam 17.00 WIB, jika telat mohon di maklumi karena saya pulang kerja juga jam 17.00 WIB.

## Index:

#### 1. Konsep Dasar

- Apa itu Python?
- Python 2.x vs 3.x
- Program Pertama Anda
- Operasi Sederhana
- Tipe Data
- Variable
- In-Place Operator

#### 2. Kontrol Struktur

- Boolean dan Persamaan
- If-Else Statements
- Logika Boolean
- While Loops
- Lists
- List Operations
- List Function
- Range
- For Loops

#### 3. Fungsi dan Modul

- Code Reuse
- Fungsi
- Argument pada Fungsi
- Pengembalian Nilai pada Fungsi
- Komentar dan Docstrings
- Fungsi sebagai Objek
- Modul
- Pustaka Standar dan PIP

#### 4. Exceptions dan Files

- Exceptions
- Exception Handling
- finnaly
- Raising Exceptions
- Assertions
- Membuka Files
- Membaca Files
- Menulis Files
- Bekerja dengan Files

#### 5. Lebih dalam dengan Data Tipe

- None
- Dictionaries
- Dictionaries Functions
- Tuples
- List Slices
- List Comprehensions
- String Formatting
- Beberapa Fungsi yang Berguna

#### 6. Functional Programming

- Intro
- Lambdas
- Map & Filters
- Generators
- Decorators
- Recursion
- Sets
- Itertools

#### 7. OOP - Object-Oriented Programming

- Classes
- Inheritance
- Magic Methods & Operator Overloading
- Object Lifecycle
- Data Hiding
- Class & Static Methods
- Properties

#### 8. Serba-serbi Python

- The Zen of Python
- PEP
- Implementasi Python
- Daftar Library Python yang Keren

#### 9. Daftar Pustaka

---

## 1. Konsep Dasar 

#### Apa itu Python?

Python adalah bahasa pemrograman interpretatif multiguna dengan filosofi perancangan yang berfokus pada tingkat keterbacaan kode. Python dikembangkan oleh Guido van Rossum pada tahun 1990 di CWI, Amsterdam sebagai kelanjutan dari bahasa pemrograman ABC. Pertama kali rilis pada tahun 1991. Python terpengaruh dari bahasa C, C++, Haskell, Java, & Perl. 

Python mendukung multi paradigma pemrograman, utamanya; namun tidak dibatasi; pada pemrograman berorientasi objek, pemrograman imperatif, dan pemrograman fungsional. Salah satu fitur yang tersedia pada Python adalah sebagai bahasa pemrograman dinamis yang dilengkapi dengan manajemen memori otomatis. Seperti halnya pada bahasa pemrograman dinamis lainnya, Python umumnya digunakan sebagai bahasa skrip meski pada praktiknya penggunaan bahasa ini lebih luas mencakup konteks pemanfaatan yang umumnya tidak dilakukan dengan menggunakan bahasa skrip. Python dapat digunakan untuk berbagai keperluan pengembangan perangkat lunak dan dapat berjalan di berbagai platform sistem operasi.

Saat ini kode Python dapat dijalankan di berbagai platform sistem operasi, beberapa di antaranya adalah: Linux/Unix, Windows, macOS, Java Virtual Machine, OS/2, Amiga, & Palm. Pada sistem operasi Linux/Unix dan macOS, secara de-facto Python sudah terinstall secara default. Namun, versi yang terinstall biasanya masih versi 2.x.

#### Python 2.x vs 3.x

Ada tiga versi major pada Python yang sekarang beredar, 1.x, 2.x, dan 3.x. Kemudian, versi ini di bagi lagi menjadi sub versi minor seperti 2.7 dan 3.5. Kedua versi Python 2.x dan 3.x masih di gunakan secara luas. Tetapi, code yang di tulis untuk versi 3.x akan di jamin kompabilitasnya untuk versi kedepannya.

Terus, apa sih bedanya Python 2.x dan 3.x ? Kenapa harus ada dualisme di antara kita ? Kenapa pengguna Python 2.x tidak move-on saja ke versi 3.x ? Ya, di balik semua itu pasti ada alasannya. Jadi begini...

Ada perubahan besar pada syntax Python versi 3.x, maka program yang di buat dengan Python 2.x tidak akan berjalan normal pada Python versi 3.x, masalah seperti ini sudah biasa dalam dunia pemrograman, dan sering di sebut “compatibility problems”. Untuk menghadapi masalah tersebut, para developer Python memberikan waktu kepada para programmer yang ‘kaget’ untuk memporting codenya ke Python 3.x dengan cara ‘masih’ memberikan support ke Python 2.x. Saat ini, status Python 2.x adalah Legacy yang artinya hanya di support seperlunya dan tidak ada pembaruan fitur terbaru (tetapi tidak menutup kemungkinan, karena Python di kembangkan oleh komunitas).

Berikut adalah bukti bahwa Python 2.x dan 3.x sangat berbeda.

Fungsi Print, pada Python 2.x

	print "tidak menggunakan tanda kurung bisa"
	print ("menggunakan tanda kurung juga bisa")
	Print "ini", ; print "mencetak satu baris"

Sedangkan Python 3.x

	print ("harus menggunakan tanda kurung")
	print ("ini digunakan untuk ", end="")
	print ("mencetak satu baris")

Jika memaksa tidak menggunakan kurung pada contoh di bawah ini:

	print "python 3 print tanpa tanda kurung"

Maka hasilnya akan error.

Itu, baru fungsi print. Masih banyak perubahan yang mendasar antara Python 2.x dan 3.x.

Lalu, versi mana yang harus di pilih ? Untuk pembuatan proyek aplikasi baru, tentu saja disarankan menggunakan versi 3.x. Walaupun ada beberapa library (pustaka) yang belum tersedia pada versi 3.x, tetapi anda jangan khawatir karena sekarang hampir semua library di situs https://pypi.python.org/pypi sudah mendukung versi 3.x.

Ayo kita install versi Python 3.x
Untuk keluarga debian dan turunannya gunakan:

	sudo apt-get install python3 python3-pip

Untuk menginstall Python 3.x di sistem operasi yang lain, silahkan google atau tanya ke member yang lain :)
Silahkan jika ada pertanyaan, atau ada yang salah mohon di benarkan :)

#### Program Pertama Anda

Pada kesempatan kali ini, kita akan membuat program pertama kita di Python. Pastikan Python yang terpasang pada sistem anda adalah versi 3.5 ke atas. Untuk memeriksa versi Python yang terpasang, gunakan perintah `python3 --version`.

Buka text editor favorit anda, seperti gedit, sublime, nano, atau vim. Kemudian ketik kode berikut pada text editor, biasakan untuk mengetik ulang setiap kode pada tutorial. Jangan hanya copy-paste, seperti kata pepatah: bisa karena terbiasa.

	#Sapa Dunia
	print ("Hallo Dunia !")
	
Kemudian, simpan dengan nama `sapa.py`. Untuk menjalankan program anda, ketik perintah `python3 sapa.py` pada terminal. Jika tidak ada pesan error, maka program anda akan mencetak teks `Hallo Dunia !` pada terminal. Selamat, anda berhasil membuat program pertama anda dengan bahasa pemrograman Python.

Selain dengan cara di atas, anda juga dapat menjalankan perintah secara langsung melalui Python Console. Untuk menjalankan python console, cukup ketik perintah `python3` pada terminal dan selanjutnya anda bisa memberikan perintah secara langsung melalui console tersebut.

#### Operasi Sederhana

Python mempunyai kemampuan untuk melakukan perhitungan matematika, untuk mencobanya silahkan masuk python console dan masukan perintah berikut 

	>>>10 + 10
	20
	>>>10 + 2 - 4
	8

Catatan: Pada python console, kode yang kita masukan di identifikasi dengan tanda `>>>` dan `...`.

Selain penambahan dan pengurangan, python juga mendukung operasi perkalian dan pembagian. Tanda bintang `*` untuk perkalian dan garis miring `/` untuk pembagian. Gunakan tanda kurung `(...)` untuk menentukan operasi yang di hitung terlebih dahulu.

	>>>5 * (2+1)
	15
	>>>20 / 5
	4.0

Catatan: Setiap operasi pembagian, maka keluaran yang di hasilkan selalu bertipe `float`. Selanjutnya, akan di jelaskan pada sesi Tipe Data.

Pada python, tanda minus pada awal bilangan menunjukan bahwa bilangan tersebut adalah bilangan negatif. Tanda plus juga bisa di berikan pada awal bilangan untuk menunjukan bahwa bilangan tersebut adalah bilangan positif, tetapi hal tersebut dirasa percuma karena tidak memberikan efek apapun, kecuali nilai keterbacaan kode.

	>>>-10
	-10
	>>>(-5) * (-10 + 3)
	35

Error juga bisa terjadi pada operasi perhitungan di python, contohnya adalah "habis dibagi nol" atau Divided by Zero.

	>>>11/0
	Traceback (most recent call last):
	File "<stdin>", line 1, in <module>
	ZeroDivisionError: division by zero
	
Hal ini terjadi karena tidak ada jawaban untuk perhitungan tersebut. Untuk menghindari kesalahan ini, selanjutya akan di bahas pada bab 4. Exceptions dan Files.

Catatan: Pada python, baris terakhir pada error menunjukan tipe dari error tersebut. Baca pesan kesalahan tersebut dengan cermat, hal ini akan membantu anda untuk memperbaiki program anda. 

#### Tipe Data

Pada python, ada beberapa tipe data yang umum di gunakan seperti `string`, `boolean`, `integer`, dan `float`.

`string` adalah tipe data yang menyatakan karakter/kalimat bisa berupa huruf angka, dll (diapit tanda `"` atau `'`). Silahkan masukan tipe data string pada python console.

	>>>"aku adalah string"
	'aku adalah string"
	
Kemudian, ada tipe data `boolean` yang menyatakan benar (`True`) yang bernilai 1, atau salah (`False`) yang bernilai 0. 

	>>>True
	True
	>>>False
	False

Untuk angka, gunakan `integer` yang menyatakan bilangan bulat. 

	>>>10
	10
	>>>15
	15
	
Sedangkan `float`, adalah tipe data yang menyatakan bilangan yang mempunyai koma. Contohnya seperti berikut.

	>>>10.5
	10.5
	>>>10.0/2
	5.0
	>>>7.7 + 2.3
	10.0
	
Itu sedikit mengenai tipe data pada python. Untuk tipe data yang lain akan di jelaskan pada Bab 5. Lebih dalam dengan Data Tipe.

#### Variable

Variable mempunyai peran yang sangat penting dalam dunia pemrograman. Variabel adalah lokasi memori yang dicadangkan untuk menyimpan nilai-nilai. Ini berarti bahwa ketika Anda membuat sebuah variabel Anda memesan beberapa ruang di memori. Variabel menyimpan data yang dilakukan selama program dieksekusi, yang natinya isi dari variabel tersebut dapat diubah oleh operasi - operasi tertentu pada program yang menggunakan variabel.

Variabel dapat menyimpan berbagai macam tipe data. Pada Python, variabel mempunyai sifat yang dinamis, artinya variabel Python tidak perlu didekralasikan tipe data tertentu dan variabel Python dapat diubah saat program dijalankan.

Penulisan variabel Python sendiri juga memiliki aturan tertentu, yaitu :

1. Karakter pertama harus berupa huruf atau garis bawah/underscore _
2. Karakter selanjutnya dapat berupa huruf, garis bawah/underscore _ atau angka
3. Karakter pada nama variabel bersifat sensitif (case-sensitif). Artinya huruf kecil dan huruf besar dibedakan. Sebagai contoh, variabel `NamaDepan` dan `namadepan` adalah variabel yang berbeda.

Untuk mulai membuat variabel di Python caranya sangat mudah, Anda cukup menuliskan variabel lalu mengisinya dengan suatu nilai dengan cara menambahkan tanda sama dengan `=` diikuti dengan nilai yang ingin dimasukan.

Dibawah ini adalah contoh penggunaan variabel dalam bahasa pemrograman Python.

	>>>IniVariable = 10
	>>>print(IniVariable)
	10
	>>>IniVariable = "Aku adalah String !"
	>>>print(IniVariable)
	Aku adalah String !
	
	>>>angka1 = 10
	>>>angka2 = 5
	>>>hasil = angka1 + angka2
	>>>print(hasil)
	15
	
	>>>NamaDepan = "Markonah"
	>>>namadepan = "Ani"
	>>>print(NamaDepan)
	Markonah
	>>>print(namadepan)
	Ani
	
	>>>_kata = "Berkata-kata"
	>>>print(_kata)
	Berkata-kata


#### In-Place Operator

In-place operators memudahkan anda untuk menulis kode menjadi lebih ringkas  `x = x + 10` menjadi `x += 10`. Selain penambahan, hal ini juga berlaku untuk operasi perhitungan yang lain seperti `+=`, `-=`, `*=`, `/=`, dan `%=`.

	>>>x = 2
	>>>print(x)
	2
	
	>>>x += 3
	>>>print(x)
	5
	
Selain operasi pada angka, operator ini juga bisa di gunakan pada tipe data lain. Contohnya pada tipe data `string`.
	
	>>>x = "telor"
	>>>print(x)
	telor
	
	>>>x += "ceplok"
	>>>print(x)
	telorceplok
---

## 2. Kontrol Struktur

#### Boolean dan Persamaan

-

#### If-Else Statements

-

#### Logika Boolean

-

#### While Loops

-

#### Lists

-

#### List Operations

-

#### List Function

-

#### Range

-

#### For Loops

-

---

## 3. Fungsi dan Modul

#### Code Reuse

-

#### Fungsi

-

#### Argument pada Fungsi

-

#### Pengembalian Nilai pada Fungsi

-

#### Komentar dan Docstrings

-

#### Fungsi sebagai Objek

-

#### Modul

-

#### Pustaka Standar dan PIP

-

---

## 4. Exceptions dan Files

#### Exceptions

-

#### Exception Handling

-

#### finnaly

-

#### Raising Exceptions

-

#### Assertions

-

#### Membuka Files

-

#### Membaca Files

-

#### Menulis Files

-

#### Bekerja dengan Files

-

---

## 5. Lebih dalam dengan Data Tipe

#### None

-

#### Dictionaries

-

#### Dictionaries Functions

-

#### Tuples

-

#### List Slices

-

#### List Comprehensions

-

#### String Formatting

-

#### Beberapa Fungsi yang Berguna

-

---

## 6. Functional Programming

#### Intro

-

#### Lambdas

-

#### Map & Filters

-

#### Generators

-

#### Decorators

-

#### Recursion

-

#### Sets

-

#### Itertools

-

---

## 7. OOP - Object-Oriented Programming

#### Classes

-

#### Inheritance

-

#### Magic Methods & Operator Overloading

-

#### Object Lifecycle

-

#### Data Hiding

-

#### Class & Static Methods

-

#### Properties

-

---

## 8. Serba-serbi Python

#### The Zen of Python

-

#### PEP

-

#### Implementasi Python

-

#### Daftar Library Python yang Keren

-

---

## 9. Daftar Pustaka

Berikut adalah sumber-sumber yang di gunakan untuk menyusun materi ini:

- http://www.belajarpython.com
- https://www.sololearn.com/
- https://docs.python.org/
- 
