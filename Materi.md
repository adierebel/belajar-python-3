# Diskusi - Awas di Makan Python !

### Disclaimer:

Materi yang di sampaikan adalah ilmu yang di serap secara otodidak, maka dari itu kesalahan sangat mungkin terjadi. Mohon di koreksi jika dirasa kurang pas atau salah. Kritik dan saran terbuka lebar, asalkan tidak out of topic. Supaya diskusi berjalan baik dan kondusif, saya akan memberikan sedikit aturan, antara lain:
1. Dilarang mengejek, menghina, atau membuat perasaan member lain tidak enak saat member tersebut mengaku tidak paham. Ayo kita bantu dia, setidaknya sampai dia paham.
2. Dilarang meragukan diri sendiri dengan berkata: “itu terlalu sulit buat saya”, dsb. Karena, melupakan ‘dia’ lebih sulit dari bahasa pemrograman apapun!
3. Materi yang di sampaikan boleh di interupsi, di kritik, atau di benarkan jika dirasa kurang pas.
4. Penyampaian materi akan di sampaikan minimal satu sub-bab setiap harinya pada jam 17.00 WIB, jika telat mohon di maklumi karena saya pulang kerja juga jam 17.00

### INDEX:

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

#### 3.Fungsi dan Modul

- Code Reuse
- Fungsi
- Argument pada Fungsi
- Pengembalian Nilai pada Fungsi
- Komentar dan Docstrings
- Fungsi sebagai Objek
- Modul
- Pustaka Standar dan PIP

#### 4.Exceptions dan Files

- Exceptions
- Exception Handling
- finnaly
- Raising Exceptions
- Assertions
- Membuka Files
- Membaca Files
- Menulis Files
- Bekerja dengan Files

#### 5.Lebih dalam dengan Data Tipe

- None
- Dictionaries
- Dictionaries Functions
- Tuples
- List Slices
- List Comprehensions
- String Formatting
- Beberapa Fungsi yang Berguna

#### 6.Functional Programming

- Intro
- Lambdas
- Map & Filters
- Generators
- Decorators
- Recursion
- Sets
- Itertools

#### 7.OOP - Object-Oriented Programming

- Classes
- Inheritance
- Magic Methods & Operator Overloading
- Object Lifecycle
- Data Hiding
- Class & Static Methods
- Properties

#### 8.Serba-serbi Python

- The Zen of Python
- PEP
- Implementasi Python
- Daftar Library Python yang Keren

---

## 1. Konsep Dasar - Apa itu Python?

Python adalah bahasa pemrograman interpretatif multiguna dengan filosofi perancangan yang berfokus pada tingkat keterbacaan kode. Python dikembangkan oleh Guido van Rossum pada tahun 1990 di CWI, Amsterdam sebagai kelanjutan dari bahasa pemrograman ABC. Pertama kali rilis pada tahun 1991. Python terpengaruh dari bahasa C, C++, Haskell, Java, & Perl. 

Python mendukung multi paradigma pemrograman, utamanya; namun tidak dibatasi; pada pemrograman berorientasi objek, pemrograman imperatif, dan pemrograman fungsional. Salah satu fitur yang tersedia pada Python adalah sebagai bahasa pemrograman dinamis yang dilengkapi dengan manajemen memori otomatis. Seperti halnya pada bahasa pemrograman dinamis lainnya, Python umumnya digunakan sebagai bahasa skrip meski pada praktiknya penggunaan bahasa ini lebih luas mencakup konteks pemanfaatan yang umumnya tidak dilakukan dengan menggunakan bahasa skrip. Python dapat digunakan untuk berbagai keperluan pengembangan perangkat lunak dan dapat berjalan di berbagai platform sistem operasi.

Saat ini kode Python dapat dijalankan di berbagai platform sistem operasi, beberapa di antaranya adalah: Linux/Unix, Windows, macOS, Java Virtual Machine, OS/2, Amiga, & Palm. Pada sistem operasi Linux/Unix dan macOS, secara de-facto Python sudah terinstall secara default. Namun, versi yang terinstall biasanya masih versi 2.x.

## 1.Konsep Dasar - Python 2.x vs 3.x

Ada tiga versi major pada Python yang sekarang beredar, 1.x, 2.x, dan 3.x. Kemudian, versi ini di bagi lagi menjadi sub versi minor seperti 2.7 dan 3.5. Kedua versi Python 2.x dan 3.x masih di gunakan secara luas. Tetapi, code yang di tulis untuk versi 3.x akan di jamin kompabilitasnya untuk versi kedepannya.

Terus, apa sih bedanya Python 2.x dan 3.x ? Kenapa harus ada dualisme di antara kita ? Kenapa pengguna Python 2.x tidak move-on saja ke versi 3.x ? Ya, di balik semua itu pasti ada alasannya. Jadi begini...

Ada perubahan besar pada syntax Python versi 3.x, maka program yang di buat dengan Python 2.x tidak akan berjalan normal pada Python versi 3.x, masalah seperti ini sudah biasa dalam dunia pemrograman, dan sering di sebut “compatibility problems”. Untuk menghadapi masalah tersebut, para developer Python memberikan waktu kepada para programmer yang ‘kaget’ untuk memporting codenya ke Python 3.x dengan cara ‘masih’ memberikan support ke Python 2.x. Saat ini, status Python 2.x adalah Legacy yang artinya hanya di support seperlunya dan tidak ada pembaruan fitur terbaru (tetapi tidak menutup kemungkinan, karena Python di kembangkan oleh komunitas).

Berikut adalah bukti bahwa Python 2.x dan 3.x sangat berbeda.

Fungsi Print, pada Python 2.x

	print “tidak menggunakan kurung bisa”
	print (“menggunakan kurung juga bisa”)
	Print “ini”, ; print “mencetak satu baris”

Sedangkan Python 3.x

	print (“harus menggunakan kurung”)
	print (“ini digunakan untuk “, end=””)
	print (“mencetak satu baris”)

jika memaksa tidak menggunakan kurung pada contoh di bawah ini:

	print "python 3 print tanpa kurung"

Maka hasilnya akan error.

Itu, baru fungsi print. Masih banyak perubahan yang mendasar antara Python 2.x dan 3.x.

Lalu, versi mana yang harus di pilih ? Untuk pembuatan aplikasi terbaru, tentu saja versi 3.x. Walaupun ada beberapa library (pustaka) yang belum tersedia pada versi 3.x, tetapi anda jangan khawatir karena sekarang hampir semua library di situs https://pypi.python.org/pypi sudah mendukung versi 3.x.

Ayo kita install versi Python 3.x
Untuk keluarga debian dan turunannya gunakan:

	sudo apt-get install python3 python3-pip

Untuk menginstall Python 3.x di sistem operasi yang lain, silahkan google atau tanya ke member yang lain :)
Silahkan jika ada pertanyaan, atau ada yang salah mohon di benarkan :)

## 1.Konsep Dasar - Program Pertama Anda

-

## 1.Konsep Dasar - Operasi Sederhana

-

## 1.Konsep Dasar - Tipe Data

-

## 1.Konsep Dasar - Variable

-

## 1.Konsep Dasar - In-Place Operator
