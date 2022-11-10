# counter_7
## Muhammad Tarreq Maulana - 2106750704 ##
## PBP B ##

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

## Readme Questions ##

1. Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget dan jelaskan perbedaan dari keduanya.

Stateless widget adalah widget pada Flutter yang tidak mempunyai state (kondisi), jadi state dari stateless widet sudah fixed dan bersifat immutable dan tidak akan berubah selama program berjalan

Stateful widget adalah widget yang berkebalikan dengan stateless widget karena besifat dinamis dan dapat berubah seiring program berjalan.


2. Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.

Widget yang digunakan pada proyek kali ini adalah:

AppBar: Menampilkan appbar dari aplikasi

Column: Agar child widget tersusun seperti sebuah kolom (ke bawah)

Text: Untuk menampilkan text apakah angka tersebut ganjil atau genap

Row: Agar child widget tersusun ke samping

FloatingActionButton: Sebagai button untuk melakukan fungsi increment/decrement pada counter

Icon: Sebagai icon yang dapat dikustomisasi pada button


3. Apa fungsi dari setState()? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.

Fungsi setState() berguna untuk mengubah tampilan UI dengan membangun ulang (rebuild) sebuah widget. Pada app ini, variabel yang terdampak dengan adanya fungsi tersebut adalah variabel _counter

4. Jelaskan perbedaan antara const dengan final.

const adalah variabel yang harus diketahui saat compile-time karena setelah diinisialisasi, variable const tersebut tidak dapat diubah. Sementara itu, final bersifat single-assignment dan apapun yang terjadi pada program tidak dapat mengubah value ataupun state dari final. Tipe final sebaiknya digunakan untuk menyimpan sesuatu yang belum diketaui saat compile-time


5. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.

Implementasi dimulai dengan membuat app flutter baru bernama counter_7. Kemudian, menambahkan fungsi untuk mengurangi variabel counter bernama _decrementCounter() dan membuat button yang ketika ditekan akan memanggil fungsi tersebut dan akan mengubah counter yang ditampilkan. Warna dari text yang ada di atas counter yang ditampilkan juga akan berubah sesuai dengan apakah angka tersebut ganjil atau genap, kemudian jika angka counter < 1, button dengan icon remove akan dihilangkan (tidak bisa decrement counter)