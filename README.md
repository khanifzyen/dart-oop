# DART Object Oriented Programming

Materi Mata Kuliah Pemrograman Mobile | Teknik Informatika UNISNU Jepara | Akhmad Khanif Zyen

OOP (Object-oriented programming) adalah metode pemrograman yang menggunakan Object dan interaksinya untuk merancang dan membuat aplikasi. OOP digunakan pada banyak bahasa pemrograman, seperti Dart, Java, C++, Python, dan lain-lain.

Keuntungan dari OOP antara lain mudah dimengerti dan digunakan, meningkatkan daya guna ulang dan mengurangi kompleksitas, meningkatkan produktivitas programmer, membuat kode lebih mudah dipelihara, dimodifikasi, dan didebug, serta mendorong kerjasama dan kolaborasi.

Fitur-fitur OOP antara lain class, object, enkapsulasi, pewarisan(inheritance), polimorfisme, dan abstraksi. OOP bertujuan untuk memecahkan masalah yang kompleks menjadi Object yang lebih kecil.

OOP dapat membuat kode menjadi lebih modular,fleksibel, dan mudah diperluas. OOP dapat membantu Anda memahami dan menyelesaikan masalah dengan lebih baik.

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
