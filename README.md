# DART Object Oriented Programming

Materi Mata Kuliah Pemrograman Mobile | Teknik Informatika UNISNU Jepara | Akhmad Khanif Zyen

OOP (Object-oriented programming) adalah metode pemrograman yang menggunakan Object dan interaksinya untuk merancang dan membuat aplikasi. OOP digunakan pada banyak bahasa pemrograman, seperti Dart, Java, C++, Python, dan lain-lain.

Keuntungan dari OOP antara lain mudah dimengerti dan digunakan, meningkatkan daya guna ulang dan mengurangi kompleksitas, meningkatkan produktivitas programmer, membuat kode lebih mudah dipelihara, dimodifikasi, dan didebug, serta mendorong kerjasama dan kolaborasi.

Fitur-fitur OOP antara lain:

1. class dan object
2. enkapsulasi (encapsulation)
3. pewarisan (inheritance)
4. polimorfisme
5. abstraksi

OOP bertujuan untuk memecahkan masalah yang kompleks menjadi Object yang lebih kecil.

OOP dapat membuat kode menjadi lebih modular,fleksibel, dan mudah diperluas. OOP dapat membantu Anda memahami dan menyelesaikan masalah dengan lebih baik.

## Konsep OOP di Dart: Class dan Object

## Class dalam Dart

Sintaks dasar class dalam Dart dimulai dengan kata kunci "class" diikuti dengan nama class. Struktur class dalam Dart terdiri dari bagian header, body, dan constructor. Header class berisi nama class dan deklarasi pewarisan (inheritance), sedangkan body class berisi properti dan method yang didefinisikan untuk class tersebut. Constructor adalah method khusus yang digunakan untuk membuat Object class tersebut.

Pembuatan Object dalam Dart dilakukan dengan menggunakan operator "=" diikuti dengan nama class dan parameter Constructor. Constructor memiliki dua jenis, yaitu Default Constructor dan Constructor dengan parameter. Default Constructor merupakan Constructor yang otomatis dibuat jika tidak didefinisikan, sedangkan Constructor dengan parameter digunakan untuk memasukkan nilai ke dalam Object.

Setiap Object yang dibuat dari class memiliki properti yang unik. Properti class dibagi menjadi dua jenis, yaitu variabel instance dan variabel statis. Variabel instance adalah variabel yang nilainya berbeda untuk setiap Object, sedangkan variabel statis nilainya sama untuk semua Object.

Method adalah fungsi khusus yang dapat digunakan untuk melakukan operasi pada Object. method juga dibagi menjadi dua jenis, yaitu method instance dan method statis. method instance dipanggil pada Object yang spesifik, sedangkan method statis dipanggil pada class itu sendiri.

Dalam pewarisan(Inheritance), class dapat mewarisi properti dan method dari class lain. Dalam Dart, konsep pewarisan ini dapat diimplementasikan dengan menggunakan kata kunci "extends". Dalam implementasinya, class turunan dapat mengakses properti dan method dari class induknya.

Untuk mendefinisikan class dalam Dart, kita menggunakan sintaks berikut:

```dart
class ClassName {
    //variable
    //method
}
```

Contoh sederhana class dalam Dart:

```dart
class Mobil {
    String? merk;
    String? model;
    int? tahun;

    void klakson(){
        print("Beep! Beep!");
    }
}
```

Dalam contoh di atas, kita mendefinisikan class Mobil dengan tiga variabel (merk, model, dan tahun) dan satu method (klakson).

Materi Mata Kuliah Pemrograman Mobile | Teknik Informatika UNISNU Jepara | Akhmad Khanif Zyen

## Membuat object dari class

Untuk membuat Object dari class, kita menggunakan sintaks berikut:

```dart
ClassName objek = ClassName();
```

Contoh membuat Object dari class Mobil:

```dart
void main(){
    Mobil mobil1 = Mobil();
}
```

Setelah Object dibuat, kita dapat mengakses variabel dan method dalam Object dengan menggunakan tanda titik (.):

```dart
void main(){
    Mobil mobil1 = Mobil();

    mobil1.merk = "Toyota";
    mobil1.model = "Corolla";
    mobil1.tahun = 2020;

    print(mobil1.merk); //Output: Toyota
    print(mobil1.model); //Output: Corolla
    print(mobil1.tahun); //Output: 2020

    mobil1.klakson(); //Output: Beep! Beep!
}
```

Dalam Dart, kita bisa menggunakan Constructor untuk membuat Object dengan nilai yang telah ditentukan. Constructor adalah method khusus yang dipanggil saat membuat Object. Berikut adalah sintaks untuk membuat Constructor dalam class:

```dart
ClassName(parameter){
    // kode konstruktor
}
```

Contoh penggunaan Constructor dalam class Mobil:

```dart
class Mobil {
    String? merk;
    String? model;
    int? tahun;

    Mobil(String merk, String model, int tahun){
        this.merk = merk;
        this.model = model;
        this.tahun = tahun;
    }

    void klakson(){
        print("Beep! Bepp!");
    }
}

void main(){
    Mobil mobil2 = Mobil("Honda","Civic",2019);

    print(mobil2.merk); //Output: Honda
    print(mobil2.model); //Output: Civic
    print(mobil2.tahun); //Output: 2019
}
```

## Kesimpulan

Class adalah elemen dasar dalam pemrograman berorientasi Object yang membantu kita mengorganisir kode dengan lebih baik. Dalam pemrograman Dart, kita dapat mendefinisikan class, membuat Object dari class, dan mengakses variabel serta method dalam Object.

Object adalah instansi dari class yang digunakan untuk mengakses variabel dan method dalam class. Dengan memahami cara kerja Object, kita dapat lebih mudah mengorganisir kode dan mengembangkan aplikasi secara efisien.

## Contoh Class & Object dalam Pemrograman Dart

### Contoh 1: class Hewan

```dart
class Hewan {
    String? nama;
    int? jumlahKaki;
    int? umur;

    void display(){
        print("Nama Hewan: $nama");
        print("Jumlah Kaki: $jumlahKaki");
        print("Umur: $umur");
    }
}

void main(){
    Hewan hewan = Hewan();
    hewan.nama = "Singa";
    hewan.jumlahKaki = 4;
    hewan.umur = 10;
    hewan.display();
}
```

Dalam contoh diatas, terdapat classs Hewan dengan tiga properti: nama, jumlahKaki, dan umur. class ini juga memiliki method display() yang mencetak nilai dari ketiga properti tersebut.

### Contoh 2: Menghitung Luas Persegi Panjang Menggunakan class dan Object

Dalam contoh di bawah ini, terdapat class PersegiPanjang dengan dua properti: panjang dan lebar. class ini juga memiliki method area() yang menghitung luas dari persegi panjang.

```dart
class PersegiPanjang {
    double? panjang;
    double? lebar;

    double area(){
        return panjang! * lebar!;
    }
}

void main(){
    PersegiPanjang persegiPanjang = PersegiPanjang();
    persegiPanjang.panjang = 10;
    persegiPanjang.lebar = 5;
    print("Luas Persegi Panjang adalah ${persegiPanjang.area()}.");
}
```

**Catatan:** Tanda seru (!) digunakan untuk memberitahu kompiler bahwa variabel tersebut tidak null. Jika Anda tidak menggunakan tanda seru, maka Anda akan mendapatkan error. Anda akan mempelajari lebih lanjut tentang null safety nanti.

### Contoh 3: Menghitung Bunga Sederhana Menggunakan class dan Object

Dalam contoh di bawah ini, terdapat class BungaSederhana dengan tiga properti: pokok, sukuBunga, dan waktu. class ini juga memiliki method bunga() yang menghitung bunga sederhana.

```dart
class BungaSederhana {
    double? pokok;
    double? sukuBunga;
    double? waktu;

    double bunga(){
        return (pokok! * sukuBunga! * waktu!) / 100;
    }
}

void main(){
    BungaSederhana bungaSederhana = BungaSederhana();
    bungaSederhana.pokok = 1000;
    bungaSederhana.sukuBunga = 10;
    bungaSederhana.waktu = 2;
    print("Bunga Sederhana adalah ${bungaSederhana.bunga()}.");
}
```

### Challenge

Buatlah class Rumah dengan properti nama, alamat, jumlahKamar. Buatlah method display() yang mencetak nilai dari ketiga properti tersebut. Buat Object dari class Rumah dan atur nilai-nilai propertinya. Panggil method display() untuk mencetak nilai dari ketiga properti tersebut.

## Constructor dalam Pemrograman Dart

Constructor adalah method khusus yang digunakan untuk menginisialisasi Object. Constructor dipanggil secara otomatis saat Object dibuat dan dapat digunakan untuk mengatur nilai awal properti Object. Sebagai contoh, kode berikut membuat Object class Orang dan mengatur nilai awal untuk properti nama dan umur.

```dart
Orang orang = Orang("Budi",30);
```

### Tanpa Constructor

Jika Anda tidak mendefinisikan Constructor untuk class, maka Anda perlu mengatur nilai properti secara manual. Sebagai contoh, kode berikut membuat Object class Orang dan mengatur nilai untuk properti nama dan umur.

```dart
Orang orang = Orang();
orang.nama = "Budi";
orang.umur = 30;
```

#### Hal-hal yang Perlu Diperhatikan

- Nama Constructor harus sama dengan nama class.
- Constructor tidak memiliki
  tipe pengembalian.

#### Sintaks:

```dart
class ClassName {
    // deklarasi konstruktor: sama dengan nama class
    ClassName() {
        // isi dari konstruktor
    }
}
```

### Contoh 1: Cara Mendeklarasikan Constructor dalam Dart

Dalam contoh di bawah ini, terdapat class Siswa dengan tiga properti: nama, umur, dan nomorInduk. class ini memiliki satu Constructor. Constructor digunakan untuk menginisialisasi nilai dari ketiga properti tersebut. Kami juga membuat Object dari class Siswa yang disebut siswa.

```dart
class Siswa {
    String? nama;
    int? umur;
    int? nomorInduk;

    // konstruktor
    Siswa(String nama, int umur, int nomorInduk){
        print("Konstruktor dipanggil");
        this.nama = nama;
        this.umur = umur;
        this.nomorInduk = nomorInduk;
    }
}

void main(){
    Siswa siswa = Siswa("Budi",30,1);
    print("Nama: ${siswa.nama}");
    print("Umur: ${siswa.umur}");
    print("Nomor Induk: ${siswa.nomorInduk}");
}
```

**Catatan:** Kata kunci this digunakan untuk merujuk ke instance saat ini dari class. Kata kunci ini digunakan untuk mengakses properti class saat ini. Dalam contoh di atas, nama parameter dan properti class dari Constructor Siswa adalah sama. Oleh karena itu, untuk menghindari kebingungan, kita menggunakan kata kunci this.

### Contoh 2: Constructor dalam Dart

Dalam contoh berikut, ada class Guru dengan empat properti: nama, umur, mataPelajaran, dan gaji. class ini memiliki satu Constructor untuk menginisialisasi nilai dari properti. class ini juga memiliki method display() yang digunakan untuk menampilkan nilai properti. Kami juga membuat 2 Object dari class Guru yang disebut guru1 dan guru2.

```dart
class Guru {
    String? nama;
    int? umur;
    String? mataPelajaran;
    double? gaji;

    //Konstruktor
    Guru(String nama, int umur, String mataPelajaran, double gaji){
        this.nama = nama;
        this.umur = umur;
        this.mataPelajaran = mataPelajaran;
        this.gaji = gaji;

    }

    //metode
    void tampilkan(){
        print("Nama: ${this.nama}");
        print("Umur: ${this.umur}");
        print("Mata Pelajaran: ${this.mataPelajaran}");
        print("Gaji: ${this.gaji}\n");// \n digunakan untuk baris baru
    }
}

void main(){
    Guru guru1 = Guru("Budi",30,"Matematika",50000.0);
    guru1.tampilkan();
    Guru guru2 = Guru("Cahyo",35,"Sains",60000.0);
    guru2.tampilkan();
}
```

Hasil keluaran:

```bash
Nama: Budi
Umur: 30
Mata Pelajaran: Matematika
Gaji: 50000

Nama: Cahyo
Umur: 35
Mata Pelajaran: Sains
Gaji: 60000
```

## Default Constructor dalam Bahasa Pemrograman Dart

Default Constructor adalah Constructor yang dibuat secara otomatis oleh kompiler Dart jika Anda tidak membuat Constructor. Default Constructor tidak memiliki parameter. Default Constructor dideklarasikan dengan menggunakan nama class diikuti dengan tanda kurung ().

### Contoh 1: Default Constructor dalam Dart

Dalam contoh berikut ini,terdapat class Laptop dengan dua properti: merek, dan harga. Mari kita buat Constructor tanpa parameter dan mencetak sesuatu dari Constructor tersebut. Kami juga memiliki Object dari class Laptop yang disebut laptop.

```dart
class Laptop {
    String? merk;
    int? harga;

    // konstruktor
    Laptop(){
        print("Ini adalah konstruktor default");
    }
}

void main(){
    //disini laptop adalah objek dari kelas Laptop
    Laptop laptop = Laptop();
}
```

## Parameterized Constructor dalam Bahasa Pemrograman Dart

Parameterized Constructor digunakan untuk menginisialisasi variabel instan dari class. Parameterized Constructor adalah Constructor yang menggunakan parameter. Constructor ini digunakan untuk mengirimkan nilai ke Constructor pada saat pembuatan Object.

```dart
class NamaKelas {
    //variabel instan
    int? angka;
    String? nama;
    //konstruktor parameter
    NamaKelas(this.angka,this.nama);
}
```

### Contoh 1: Parameterized Constructor dalam Dart

Dalam contoh di bawah ini, terdapat class Student dengan tiga properti: name, age, dan rollNumber. class ini memiliki satu Constructor. Constructor ini digunakan untuk menginisialisasi nilai dari ketiga properti tersebut. Kami juga memiliki Object dari class Student yang disebut student.

```dart
class Student {
    String? name;
    int? age;
    int? rollNumber;

    //konstruktor
    Student(this.name, this.age, this.rollNumber);
}

void main(){
    //disini student adalah object dari class Student
    Student student = Student("John", 20, 1);
    print("Name: ${student.name}");
    print("Age: ${student.age}");
    print("Roll Number: ${student.rollNumber}");
}
```

Hasil keluaran:

```bash
Name: John
Age: 20
Roll Number: 1
```

### Contoh 2: Parameterized Constructor dengan Parameter Bernama dalam Dart

Dalam contoh di bawah ini, terdapat class Student dengan tiga properti: name, age, dan rollNumber. class ini memiliki satu Constructor. Constructor ini digunakan untuk menginisialisasi nilai dari ketiga properti tersebut. Kami juga memiliki Object dari class Student yang disebut student.

```dart
class Student {
    String? name;
    int? age;
    int? rollNumber;

    //konstruktor
    Student({String? name, int?age, int? rollNumber}){
        this.name = name;
        this.age = age;
        this.rollNumber = rollNumber;
    }
}

void main(){
    //disini student adalah object dari class Student
    Student student = Student(name: "John", age: 20, rollNumber: 1);
    print("Name: ${student.name}");
    print("Age: ${student.age}");
    print("Roll Number: ${student.rollNumber}");
}
```

Hasil keluaran:

```bash
Name: John
Age: 20
Roll Number: 1
```

### Contoh 3: Parameterized Constructor dengan Nilai Default dalam Dart

Dalam contoh di bawah ini, terdapat class Student dengan dua properti: name, dan age. class ini memiliki Parameterized Constructor dengan nilai default. Constructor ini digunakan untuk menginisialisasi nilai dari kedua properti tersebut. Kami juga memiliki Object dari class Student yang disebut student.

```dart
class Student {
    String? name;
    int? age;

    //konstruktor
    Student({String? name = "John",int? age = 0}){
        this.name = name;
        this.age = age;
    }
}

void main(){
    //disini student adalah object dari class Student
    Student student = Student();
    print("Name: ${student.name}");
    print("Age: ${student.age}");
}
```

Hasil keluaran:

```bash
Name: John
Age: 0
```

## Named Constructor dalam Dart

Dalam kebanyakan bahasa pemrograman seperti Java, C++, C#, dll., kita bisa membuat beberapa Constructor dengan nama yang sama. Namun dalam Dart, hal ini tidak mungkin. Tetapi ada cara lain, kita bisa membuat beberapa Constructor dengan nama yang sama menggunakan Named Constructor.

**Catatan:** Named Constructor meningkatkan keterbacaan kode. Ini berguna ketika Anda ingin membuat beberapa Constructor dengan nama yang sama.

### Contoh 1: Named Constructor dalam Dart

Dalam contoh di bawah ini, ada class Student dengan tiga properti: name, age, dan rollNumber. class ini memiliki dua Constructor. Constructor pertama adalah Default Constructor. Constructor kedua adalah Named Constructor. Named Constructor digunakan untuk menginisialisasi nilai ketiga properti. Kami juga memiliki Object dari class Student yang disebut student.

```dart
class Student {
    String? name;
    int? age;
    int? rollNumber;

    //default constructor
    Student(){
        print("This is a default constructor");
    }

    //named constuctor
    Student.namedConstructor(String name, int age, int rollNumber){
        this.name = name;
        this.age = age;
        this.rollNumber = rollNumber;
    }
}

void main(){
    //disini student adalah object dari class Student
    Student student = Student.namedConstructor("John", 20, 1);
    print("Name: ${student.name}");
    print("Age: ${student.age}");
    print("Roll Number: ${student.rollNumber}");
}
```

Hasil keluaran:

```
Name: John
Age: 20
Roll Number: 1
```

### Contoh 2: Named Constructor dalam Dart

Dalam contoh di bawah ini, ada class Mobile dengan tiga properti name, color, dan prize. Class ini memiliki satu method display yang mencetak nilai ketiga properti. Kami juga memiliki Object dari class Mobile yang disebut mobile. Ada juga Constructor Mobile yang mengambil ketiga properti sebagai parameter. Named Constructor Mobile.namedConstructor digunakan untuk membuat Object dari class Mobile dengan name, color dan prize opsional. Nilai default dari prize adalah 0. Jika prize tidak dilewatkan, maka nilai default akan digunakan.

```dart
class Mobile {
    String? name;
    String? color;
    int? prize;

    Mobile(this.name, this.color, this.prize);

    //disini Mobile() adalah named constructor
    Mobile.namedConstructor(this.name, this.color, [this.prize=0]);

    void displayMobileDetails(){
        print("Mobile name: $name.");
        print("Mobile color: $color.");
        print("Mobile prize: $prize\n");
    }
}

void main(){
    var mobile1 = Mobile("Samsung", "Black",20000);
    mobile1.displayMobileDetails();
    var mobile2 = Mobile.namedConstructor("Apple", "White");
    mobile2.displayMobileDetails();
}
```

Hasil keluaran:

```bash
Mobile name: Samsung.
Mobile color: Black.
Mobile prize: 20000

Mobile name: Apple.
Mobile color: White.
Mobile prize: 0
```

### Contoh 3: Named Constructor dalam Dart

Dalam contoh di bawah ini, ada class Animal dengan dua properti name dan age. class ini memiliki tiga Constructor. Constructor pertama adalah Default Constructor. Constructor kedua dan ketiga adalah Named Constructor. Constructor kedua digunakan untuk menginisialisasi nilai name dan age, dan Constructor ketiga digunakan untuk menginisialisasi nilai name saja. Kami juga memiliki Object dari class Animal yang disebut animal.

```dart
class Animal {
    String? name;
    int? age;

    //default constructor
    Animal(){
        print("Ini adalah default constructor");
    }

    //named constructor
    Animal.namedConstructor(String name, int age){
        this.name = name;
        this.age = age;
    }

    //named constructor
    Animal.namedConstructor2(String name){
        this.name = name;
    }
}

void main(){
    //disini animal adalah object dari class Animal
    Animal animal = Animal.namedConstructor("Dog", 5);
    print("Name: ${animal.name}");
    print("Age: ${animal.age}");

    Animal animal2 = Animal.namedConstructor2("Cat");
    print("Name: ${animal2.name}");
}
```

Hasil keluaran:

```bash
Name: Dog
Age: 5
Name: Cat
```

### Contoh 4: Contoh Nyata Named Constructor dalam dart

Dalam contoh di bawah ini, ada class Person dengan dua properti name dan age. class ini memiliki tiga Constructor. Constructor pertama adalah Parameterized Constructorisasi yang mengambil dua parameter name dan age. Constructor kedua dan ketiga adalah Named Constructor. Constructor kedua fromJson digunakan untuk membuat Object dari class Person dari JSON. Constructor ketiga fromJsonString digunakan untuk membuat Object dari class Person dari string JSON. Kami juga memiliki Object dari class Person yang disebut person.

```dart
import 'dart:convert';

class Person {
    String? name;
    int? age;

    Person(this.name, this.age);

    Person.fromJson(Map<String, dynamic> json){
        name = json['name'];
        age = json['age'];
    }

    Person.fromJsonString(String jsonString){
        Map<String, dynamic> json = jsonDecode(jsonString);
        name = json['name'];
        age = json['age'];
    }
}

void main(){
    //disini person adalah object dari class Person
    String jsonString1 = '{"name": "Agus", "age": 20}';
    String jsonString2 = '{"name": "Budi", "age": 25}';

    Person p1 = Person.fromJsonString(jsonString1);
    print("Person 1 name: ${p1.name}");
    print("Person 1 age: ${p1.age}\n");

    Person p2 = Person.fromJsonString(jsonString2);
    print("Person 2 name: ${p2.name}");
    print("Person 2 age: ${p2.age}");
}
```

Hasil keluaran:

```bash
Person 1 name: Agus
Person 1 age: 20

Person 2 name: Budi
Person 2 age: 25
```

## Constant Constructor dalam Dart

Constant Constructor adalah Constructor yang menciptakan Object konstan. Object konstan adalah Object yang nilai tidak dapat diubah. Constant Constructor dideklarasikan dengan menggunakan kata kunci const.

**Catatan:** Constant Constructor digunakan untuk membuat Object yang
nilainya tidak dapat diubah. Ini meningkatkan kinerja program.

Aturan untuk Mendeklarasikan Constant Constructor dalam Dart:

- Semua properti class harus final.
- Tidak memiliki badan.
- Hanya class yang mengandung Constructor const diinisialisasi menggunakan kata kunci const.

### Contoh 1: Constant Constructor dalam Dart

Dalam contoh di bawah ini, ada class Point dengan dua properti final: x dan y. class ini juga memiliki Constant Constructor yang menginisialisasi dua properti tersebut.

```dart
class Point {
    final int x;
    final int y;

    const Point(this.x, this.y);
}

void main(){
    //p1 dan p2 memiliki kode hash yang sama
    Point p1 = const Point(1, 2);
    print("Kode hash p1 adalah: ${p1.hashCode}");

    Point p2 = const Point(1, 2);
    print("Kode hash p2 adalah: ${p2.hashCode}");

    // tanpa menggunakan const
    // ini memiliki kode hash yang berbeda
    Point p3 = Point(2, 2);
    print("Kode hash p3 adalah: ${p3.hashCode}");

    Point p4 = Point(2, 2);
    print("Kode hash p4 adalah: ${p4.hashCode}");
}
```

Hasil keluaran:

```bash
Kode hash p1 adalah: 248788600
Kode hash p2 adalah: 248788600
Kode hash p3 adalah: 533057249
Kode hash p4 adalah: 683584498
```

**Catatan:** Di sini p1 dan p2 memiliki kode hash yang sama. Ini karena p1 dan p2 adalah Object konstan. Kode hash dari Object konstan sama. Ini karena kode hash dari Object konstan dihitung saat waktu kompilasi. Kode hash dari Object non-konstan dihitung saat waktu runtime. Inilah mengapa p3 dan p4 memiliki kode hash yang berbeda.

### Contoh 2: Constant Constructor dalam Dart

Dalam contoh di bawah ini, ada class Student dengan tiga properti: name, age, dan rollNumber. class ini memiliki satu Constant Constructor. Constructor ini digunakan untuk menginisialisasi nilai dari ketiga properti tersebut. Kami juga memiliki Object dari class Student yang disebut student.

```dart
class Student {
    final String? name;
    final int? age;
    final int? rollNumber;

    //Constant Constructor
    const Student({this.name, this.age, this.rollNumber});
}

void main(){
    //disini student adalah object dari class Student
    const Student student = Student(name: "Budi", age: 28, rollNumber: 1);
    print("Name: ${student.name}");
    print("Age: ${student.age}");
    print("Roll Number: ${student.rollNumber}");
}
```

Hasil keluaran:

```bash
Name: Budi
Age: 28
Roll Number: 1
```

### Contoh 3: Constant Constructor dengan Parameter Bernama dalam Dart

Dalam contoh di bawah ini, ada class Car dengan tiga properti: name, model, dan prize. class ini memiliki satu Constructor. Constructor ini digunakan untuk menginisialisasi nilai dari ketiga properti tersebut. Kami juga memiliki Object dari class Car yang disebut car.

```dart
class Car {
    final String? name;
    final String? model;
    final int? prize;

    //constant constructor
    const Car({this.name, this.model, this.prize});
}

void main(){
    //disini car adalah object dari class Car
    const Car car = Car(name: "BMW", model: "X5", prize: 50000);
    print("Name: ${car.name}");
    print("Model: ${car.model}");
    print("Prize: ${car.prize}");
}
```

Hasil keluaran:

```bash
Name: BMW
Model: X5
Prize: 50000
```

> **Tugas Latihan 1**
>
> 1. Buatlah sebuah class Mobil dalam Dart yang memiliki properti seperti merk, model, dan tahun. Selanjutnya, buat objek dari class tersebut dan inisialisasikan dengan nilai tertentu. Cetak informasi mobil tersebut.
> 2. Buatlah class Mahasiswa dengan properti nama dan nim. Berikan nilai default untuk kedua properti tersebut. Buat objek dari class Mahasiswa tanpa memberikan nilai tambahan, dan cetak informasi mahasiswa tersebut.
> 3. Buat class Buku dengan properti judul dan pengarang. Implementasikan parameterized constructor untuk menginisialisasi properti saat objek dibuat. Buat objek dari class Buku dengan memberikan nilai pada konstruktor, dan cetak informasi buku tersebut.
> 4. Buat class Segitiga dengan properti alas, tinggi, dan jenis (contoh: siku-siku, sama sisi, dsb.). Implementasikan named constructor untuk membuat objek Segitiga berdasarkan jenisnya. Buat objek dari class Segitiga menggunakan named constructor, dan cetak informasi segitiga tersebut.
> 5. Buat class Warna dengan properti red, green, dan blue. Implementasikan constant constructor untuk menginisialisasi warna yang bersifat konstan. Buat beberapa objek dari class Warna menggunakan constant constructor, dan cetak informasi warna-warna tersebut.

## Konsep OOP di Dart: Encapsulation

Encapsulation adalah salah satu prinsip dasar dalam pemrograman berorientasi objek (OOP) yang menggabungkan data dan metode yang beroperasi pada data ke dalam sebuah unit tunggal, yang disebut class. Dengan menggunakan encapsulation, kita dapat menyembunyikan rincian implementasi internal suatu objek dan hanya mengekspos fungsionalitas yang diperlukan.

### Bagaimana menerapkan encapsulation dalam OOP di dart?

Cara mudahnya adalah dengan melakukan hal berikut:

1. menjadikan property di dalam class menjadi private dengan menambahkan underscore (\_)
2. membuat method setter dan getter untuk mengakses dan mengupdate property private tersebut

Pada materi membuat object pada class OOP di dart sebelumnya, anda membuat property secara public, sehingga class / object eksternal lain bisa dengan leluasa langsung mengganti property dari object tersebut. Ini akan menjadi resiko tersendiri.

### Sehingga didapatkan tujuan dari encapsulation yaitu:

- **Penyembunyian Data:** Encapsulation menyembunyikan data dari dunia luar. Ini mencegah data diakses oleh kode di luar class. Ini dikenal sebagai penyembunyian data.
- **Mudah di-testing**: Encapsulation memungkinkan Anda menguji class secara terisolasi. Ini akan memungkinkan Anda menguji kelas tanpa menguji kode di luar kelas.
- **Fleksibilitas:** Encapsulation memungkinkan Anda mengubah implementasi class tanpa mempengaruhi kode di luar kelas.
- **Keamanan:** Encapsulation memungkinkan Anda membatasi akses ke anggota class. Ini akan memungkinkan Anda membatasi akses ke anggota class dari kode di luar library.

### Contoh 1: Encapsulation di dart

```dart
class Employee {
  // property private
  int? _id;
  String? _name;

// Method getter untuk mengakses property private _id
  int getId() {
    return _id!;
  }
// Method getter untuk mengakses property private _name
  String getName() {
    return _name!;
  }
// Method setter untuk meng-update property private _id
  void setId(int id) {
    this._id = id;
  }
// Method setter untuk meng-update property private _name
  void setName(String name) {
    this._name = name;
  }

}

void main() {
  // Membuat object dari class Employee
  Employee employee = new Employee();
  // Memberi nilai ke object menggunakan setter
  employee.setId(1);
  employee.setName("John");

  // Menerima nilai dari object menggunakan getter
  print("Id: ${employee.getId()}");
  print("Name: ${employee.getName()}");
}
```

Sekarang coba kamu akses property langsung dari object dengan cara seperti berikut:

```dart
...
void main() {
  var employee = Employee();
  employee._name = "John"; // Bisa berfungsi dan tidak eror, tapi kenapa?
  print(employee.getName());
}
```

Alasannya adalah penggunaan underscore (\_) sebelum nama variabel atau method membuatnya menjadi **private library**, bukan **private class**. Ini berarti bahwa variabel atau method hanya terlihat oleh library tempat itu dideklarasikan. Ini tidak terlihat oleh library lain. Dengan kata lain, library adalah satu file. Jika Anda menulis method utama di file terpisah, ini tidak akan berfungsi.

**Solusi:** Untuk melihat private property beraksi, Anda harus membuat file terpisah untuk class tersebut dan mengimpornya ke dalam file utama (yang memiliki fungsi `main()`).

### Contoh 2: Encapsulation menggunakan keyword get dan set

Selain membuat method buatan sendiri seperti `setId()`, `getId()` dan seterusnya, anda bisa menggunakan setter dan getter bawaan dart seperti contoh berikut:

```dart
class Vehicle {
  String _model;
  int _year;

  // Getter method
  String get model => _model;

  // Setter method
  set model(String model) => _model = model;

  // Getter method
  int get year => _year;

  // Setter method
  set year(int year) => _year = year;
}

void main() {
  var vehicle = Vehicle();
  vehicle.model = "Toyota";
  vehicle.year = 2019;
  print(vehicle.model);
  print(vehicle.year);
}
```

## Konsep OOP di Dart: Inheritance

Inheritance atau pewarisan adalah konsep dalam pemrograman berorientasi objek (OOP) di mana sebuah class dapat mewarisi properti dan metode dari class lain. Class yang mewarisi disebut subclass atau child class, sedangkan class yang memberikan warisan disebut superclass atau parent class. Menggunakan keyword `extends` untuk menerima warisan dari parent class.

### Sintaks:

```dart
class ParentClass {
  // Parent class code
}

class ChildClass extends ParentClass {
  // Child class code
}
```

**Catatan:** Setiap kali Anda menggunakan pewarisan, ia selalu membuat hubungan "adalah" antara class induk dan anak, seperti **Mahasiswa adalah Orang**, **Truk adalah Kendaraan**, **Sapi adalah Hewan**, dan sebagainya.

Dart mendukung inheritance tunggal, berarti class anak hanya bisa mewarisi dari satu class induk. Dart tidak mendukung multi inheritance yang berarti class anak tidak dapat mewarisi dari beberapa class induk.

### Tujuan inheritance:

- Penggunaan Kembali Kode (Code Reusability): Menghindari duplikasi kode dengan menggunakan properti dan metode yang sudah ada.
- Struktur Hirarki: Membentuk struktur hierarki antara class.

### Contoh 1: Inheritance di dart

```dart
// Parent Class
class Binatang {
  String jenis;

  Binatang(this.jenis);

  void bersuara() {
    print('Sebuah binatang dari jenis $jenis bersuara.');
  }
}

// Child Class yang mewarisi dari Binatang
class Kucing extends Binatang {
  String jenisBulu;

  Kucing(String jenis, this.jenisBulu) : super(jenis);

  void tidur() {
    print('Kucing tidur dengan nyenyak.');
  }
}
```

### Penggunaan keyword `super`

Keyword `super` digunakan untuk merujuk ke superclass (parent class). Dalam contoh di atas, `super(jenis)` digunakan untuk memanggil constructor dari superclass saat membuat objek dari subclass.

### Contoh 2: Inheritance di dart

```dart
class Orang {
  // Property
  String? nama;
  int? umur;

  // Method
  void tampil() {
    print("Nama: $nama");
    print("Umur: $umur");
  }
}
// Disini class Murid akan mewarisi property dan method dari class Orang
class Murid extends Orang {
  // property
  String? namaSekolah;
  String? alamatSekolah;

  // Method
  void tampilInfoSekolah() {
    print("Nama Sekolah: $namaSekolah");
    print("Alamat Sekolah: $alamatSekolah");
  }
}

void main() {
  // Membuat object dari class Murid
  var murid = Murid();
  murid.nama = "Joko";
  murid.umur = 16;
  murid.namaSekolah = "SMA N 1";
  murid.alamatSekolah = "Jepara";
  murid.tampil();
  murid.tampilInfoSekolah();
}
```

### Jenis inheritance

1. single inheritance: pewarisan dari satu ParentClass ke satu ChildClass

```
  -- Kendaraan     // class Kendaraan
     |-- Mobil     // class Mobil extends Kendaraan
```

2. multilevel inheritance:pewarisan dari satu ParentClass ke satu ChildClass kemudian ke bawah subclassnya lagi.

```
  -- Kendaraan     // class Kendaraan
     |-- Mobil     // class Mobil extends Kendaraan
         |-- Tesla // class Tesla extends Mobil
```

3. hierachical inheritance: pewarisan dari satu ParentClass ke dua ChildClass

```
  -- Kendaraan     // class Kendaraan
     |-- Mobil     // class Mobil extends Kendaraan
     |-- Motor     // class Motor extends Kendaraan
```

4. multiple inheritance: pewarisan dari dua ParentClass atau lebih ke satu ChildClass. **Ini tidak didukung oleh dart.**

```
  -- Buah           // class Buah
  -- Sayuran        // class Sayuran
     |-- Tomat      // class Tomat extends Buah, Sayuran
```

### Contoh 3: Multilevel Inheritance di dart

```dart
class Mobil {
    // Property
    String? nama;
    double? harga;
}

class Tesla extends Mobil {
    // Method untuk menampilkan nilai dari property
    void tampil() {
        print("Nama: ${nama}");
        print("Harga: ${harga}");
    }
}

class Model3 extends Tesla {
    // Property
    String? warna;

    // Method untuk menampilkan nilai dari property
    void tampil() {
        super.tampil();
        print("Warna: ${warna}");
    }
}

void main() {
    // Membuat object dari class Model3
    Model3 m = new Model3();
    // memberikan nilai ke object
    m.nama = "Tesla Model 3";
    m.harga = 50000.00;
    m.warna = "Merah";
    // Menampilkan nilai dari object
    m.tampil();
}
```

### Contoh 4: Hierarchical Inherintance di dart

```dart
class Bangun {
  // Properties
  double? diameter1;
  double? diameter2;
}

class Lingkaran extends Bangun {
  // Method untuk menghitung luas lingkaran
  double luas() {
    return 3.14 * diameter1! * diameter2!;
  }
}

class Segitiga extends Bangun {
  // Method untuk menghitung luas segitiga
  double luas() {
    return 0.5 * diameter1! * diameter2!;
  }
}

void main() {
  // Membuat object dari class Lingkaran
  Lingkaran lingkaran = new Lingkaran();
  // memberikan nilai diameter ke object
  lingkaran.diameter1 = 10.0;
  lingkaran.diameter2 = 20.0;
  // Tampilkan luas dari lingkaran
  print("Luas lingkaran: ${lingkaran.luas()}");

  // Membuat object dari class Segitiga
  Segitiga segitiga = new Segitiga();
  // memberikan nilai ke object
  segitiga.diameter1 = 10.0;
  segitiga.diameter2 = 20.0;
  // Tampilkan luas segigita
  print("Luas segitiga: ${segitiga.luas()}");
}
```