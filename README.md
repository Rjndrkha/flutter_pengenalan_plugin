# flutter_pengenalan_plugin
___

## Langkah 1 || Buat Project Baru && Langkah 2 || Menambahkan Plugin
Menambahkan plugin auto_size_text agar dapat diimport
![Screenshot (2513)](https://user-images.githubusercontent.com/75615789/188351115-89d0bb27-ccf2-4023-8ef6-37071aa6b704.png)

## Langkah 3 || Buat file red_text_widget.dart && Langkah 4 || Tambah Widget AutoSizeText
Masih di file red_text_widget.dart, untuk menggunakan plugin auto_size_text ubah kode return
![Screenshot (2514)](https://user-images.githubusercontent.com/75615789/188351716-9bbfba61-e82c-4b12-881d-951b9a787dff.png)


## Langkah 5 || Buat Variabel text dan parameter di constructor
Agar Tidak eror ditambahkan variabel text kedalam parameter di construktor
![Screenshot (2515)](https://user-images.githubusercontent.com/75615789/188352015-1596acfe-8341-4f7a-bd8c-d168b07868e7.png)

## Langkah 6 || Tambahkan widget di main.dart
Modifikasi Program Agar tampilan lebih menarik 
![Screenshot (2516)](https://user-images.githubusercontent.com/75615789/188353173-c53c5f6a-d4ce-4f12-a1cd-6ec187ce0196.png)

___

# Tugas Praktikum

## Jelaskan maksud dari langkah 2 pada praktikum tersebut!
```
'flutter pub add auto_size_text' 

Jadi maksud dari code tersebut adalah untuk Mendownload package flutter auto_size_text kemudian akan otomatis ditambahkan di pubspec.yaml

```
## Jelaskan maksud dari langkah 5 pada praktikum tersebut!
```
child: const RedTextWidget(
             text: 'You have pushed the button this many times:',
          ),

Agar text tersebut dapat dipanggil di class main.dart kita harus menambahkan construktor terlebih dahulu agar nantinya value nya dapat terisi. dan karena
text jadi untuk tipe data nya kita menggunakan final String text;
```
## Pada langkah 6 terdapat dua widget yang ditambahkan, jelaskan fungsi dan perbedaannya!
```
Container(
   color: Colors.yellowAccent,
   width: 50,
   child: const RedTextWidget(
             text: 'You have pushed the button this many times:',
          ),
),

Pada widget diatas adalah pemanggilan fungsi class dari RedTextWidget Yang telah ditambahkan , Kemudian Untuk Perbedaan yang menggunakan package 
text lebih terlihat rapi

Container(
    color: Colors.greenAccent,
    width: 100,
    child: const Text(
           'You have pushed the button this many times:',
          ),
),

Pada widget diatas adalah widget biasa tanpa menggunakan package apapun , code diatas menggunakan default text widget
Perbedaanya seperti dibawah ini :
```
![Screenshot (2516)](https://user-images.githubusercontent.com/75615789/188353173-c53c5f6a-d4ce-4f12-a1cd-6ec187ce0196.png)

## Jelaskan maksud dari tiap parameter yang ada di dalam plugin auto_size_text berdasarkan tautan pada dokumentasi [ini](https://pub.dev/documentation/auto_size_text/latest/) !

```
auto size text terbagi dalam beberapa Fungsi : 

1. Auto Size Max Lines
> Jumlah maksimum baris opsional untuk teks yang akan dibentangkan.

2. minFontSize & maxFontSize
> minFontSize : Batasan ukuran teks minimum yang akan digunakan saat mengubah ukuran teks secara otomatis.
Diabaikan jika presetFontSizesdisetel.
> maxFontSize : Batasan ukuran teks maksimum yang akan digunakan saat mengubah ukuran teks secara otomatis.
Diabaikan jika presetFontSizesdisetel.

3. Auto Size
> Batasan ukuran teks minimum yang akan digunakan saat mengubah ukuran teks secara otomatis.
Diabaikan jika presetFontSizesdisetel.
> Batasan ukuran teks maksimum yang akan digunakan saat mengubah ukuran teks secara otomatis.
Diabaikan jika presetFontSizesdisetel.

4. stepGranularity
> Ukuran langkah di mana ukuran font sedang disesuaikan dengan batasan.

5. OverflowReplacement
> Jika teks meluap dan tidak sesuai dengan batasnya, widget ini akan ditampilkan sebagai gantinya.
```
