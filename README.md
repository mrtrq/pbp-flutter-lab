# pbp-flutter-lab

## Repository ini berisikan tugas Platfrom Based Programming yang dipelajari di semester 3 selama perkuliahan di Fakultas Ilmu Komputer UI (Fasilkom).
---
### Topik pembelajaran kali ini adalah terkait Flutter. Pada tutorial sebelumnya, kita telah menginstall Flutter. Setelah menginstall dan membuat app, kita langsung diperlihatkan dengan demonstasi counter yang dapat ditambah. Pada tugas 7, kita diminta untuk membuat tombol + dan - dan menentukan apakah bilangan tersebut merupakan bilangan ganjil atau genap.

----
# Tugas Kedua Flutter - Flutter Form  #

### 1. Jelaskan perbedaan Navigator.push dan Navigator.pushReplacement.

Perbedaan antara Navigator.push dan Navigator.pushReplacement adalah jumlah routing pada stack Navigator. Pada .push, jumlah routing di dalam stack akan bertambah. Namun, ketika .pushReplacement, route yang akan dituju akan menggantikan route sebelumnya di stack (mirip seperti pop pada stack)


### 2. Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.

Terdapat widgets yang telah digunakan pada tugas sebelumnya, yaitu counter sederhana di tugas 7, kemudian terdapat  widget tambahan, yaitu:

* Drawer

Widget ini dipergunakan untuk menyediakan drawer atau hamburger menu untuk tombol menuju routing page yang lain.

* Navigator

Bertindak untuk menuju ke routing yuang lain. Bisa menggunakan Navigator.push dan Navigator.pushReplacement.

* ListTile

Semacam container yang memiliki tinggi yang fixed yang dapat berisikan text. Digunakan sebagai tombol terhadap page lain.

* Form

Suatu container untuk mewadahi bermacam widget form. Digunakan pada form.dart

* TextFormField

Merupakan suatu field untuk menerima input berupa teks. Pada tugas kali ini dimanfaatkan untuk menerima input judul dan nominal budget.

* DropdownButtonField

Merupakan suatu field yang menyediakan dropdown agar user dapat memilih opsi. Digunakan untuk menyediakan pilihan jenis budget.

* TextButton

Kasarnya button yang dapat ditekan dan memiliki fungsi setelah ditekan. Digunakan sebagai tombol submit dari form budget.

* Card

Sebuah panel yang bisa digunakan untuk menunjukkan informasi atau text. Pada tugas ini digunakan untuk menampilkan data dari budget.



### 3. Sebutkan jenis-jenis event yang ada pada Flutter (contoh: onPressed).
Beberapa jenis-jenis event yang ada pada Flutter adalah onPressed, onChanged, onSaved, onTap, onHover

### 4. Jelaskan bagaimana cara kerja Navigator dalam "mengganti" halaman dari aplikasi Flutter.

Navigator mengganti halaman dengan menyimpan navigasi-nagivasi tersebut dalam sebuah stack, kemudian untuk pindah ke halaman lain, dapat menggunakana Navigator.push ataupun Navigator.pop. 

.push digunakan untuk berpindah ke halaman baru sementara .pop dapat digunakan untuk berpindah ke halaman yang sebleumnya

### 5. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
1. Membuat widget drawer pada navbar sebagai sarana untuk bernavigasi pada aplikasi (berpindah ke halaman Counter, Tambah Budget, dan Data Budget) dengan membuat file drawer.dart

2. Membuat file baru bernama form.dart yang merupakan halaman form untuk memproses tambah budget. Setiap budget yang ditambahkan akan disimpan dalam list.

3. Membuat file baru bernama data.dart yang merupakan halaman untuk menampilkan budget-budget yang ditambahkan.

4. import file-file lainnya di folder lib, kemudian membuat fungsi yang mengembalikan Drawer(), dan lakukan drawer: returnMyDrawer(context),