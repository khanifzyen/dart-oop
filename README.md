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
    String merk;
    String model;
    int tahun;

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
    doub
}
```
