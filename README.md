# UTS Pemrograman Mobile 2

Nama              : Amanda Puspa Negara

NIM               : 312210129

Kelas             : TI.22 C.1

Mata Kuliah       : Pemrograman Mobile 2

Dosen Pengampu    : Eko Budiarto S.kom., M.M.

# Perintah Tugas

Perintah tugas kali ini adalah mengumpulkan semua hasil yang sudah dibuat dari module hal 30-72 digabungkan dalam satu Aplikasi. Berikut ini semua code yang telah saya buat.

# Penjelasan Aplikasi

Sebelumnya saya akan menjelaskan terlebih dahulu, ada apa saja didalam aplikasi ini. Berikut ini adalah daftarnya :

- Hello World , di activity ini adalah awal dari pengenalan terhadap software Flutter. Didalam activity ini hanya terdapat kalimat yang bertuliskan "Hello World"
- Widget Column ,  activity ini Column biasanya digunakan untuk membuat Form
- Widget Row , activity ini Untuk menampilkan Widget dalam posisi horizontal dapat menggunakan Widget Row.
- Form ,  agar lebih rapi untuk tampilan halaman akan kita kelompokkan
- Detail Produk 
- ListView Produk 

# Source Code

Disini saya tidak akan menampilkan source codenya disini, karena akan terlalu banyak dan memakan tempat dan hanya membuat pusing melihatnya. Saya sudah push semua file dari project yang sudah saya buat dan jika menginginkan bisa mendownload beberapa file yang dibutuhkan saja atau clone repository ini sepenuhnya. Sebagai gantinya, saya hanya akan menjelaskan sedikit dari apa saja yang sudah saya kerjakan.

A. Source Code Utama

- main.dart [Lihat File](aplikasi_flutter_pertamaku/lib/main.dart)<br>

Di Main.dart ini berisi program yang memiliki fungsi penghubung dari semua project yang ada. Saya beri nama file ini Main karena disinilah fungsi paling awal dari halaman awal.


B. Hello World

- helloworld.dart [Lihat File](aplikasi_flutter_pertamaku/lib/hello_world.dart)<br>

main.dart untuk hello world
       
        import 'package:flutter/material.dart';
        
        void main() {
          runApp(const MyApp());
        }
        
        class MyApp extends StatelessWidget {
          const MyApp({Key? key}) : super(key: key);
        
          @override
          Widget build(BuildContext context) {
            return MaterialApp(
              title: "Aplikasi Flutter Pertama",
              home: HelloWorld(),
            );
          }
        }

C. Widget Column

- column_widget.dart [Lihat File](aplikasi_flutter_pertamaku/lib/column_widget.dart)<br>

main.dart untuk Widget Column

        import 'package:flutter/material.dart';
        
        void main() {
          runApp(const MyApp());
        }
        
        class MyApp extends StatelessWidget {
          const MyApp({Key? key}) : super(key: key);
        
          @override
          Widget build(BuildContext context) {
            return MaterialApp(
              title: "Aplikasi Flutter Pertama",
              home: ColumnWidget(),
            );
          }
        }
        
D. Row Widget

- row_widget.dart [Lihat File](aplikasi_flutter_pertamaku/lib/row_widget.dart
)<br>

main.dart untuk Row Widget

        import 'package:flutter/material.dart';
        
        void main() {
          runApp(const MyApp());
        }
        
        class MyApp extends StatelessWidget {
          const MyApp({Key? key}) : super(key: key);
        
          @override
          Widget build(BuildContext context) {
            return MaterialApp(
              title: "Aplikasi Flutter Pertama",
              home: RowWdget(),
            );
          }
        }

E. Produk Form

- produk_form.dart [Lihat File](aplikasi_flutter_pertamaku/lib/ui/produk_form.dart)<br>

main.dart untuk Produk Form

        import 'package:flutter/material.dart';
        
        void main() {
          runApp(const MyApp());
        }
        
        class MyApp extends StatelessWidget {
          const MyApp({Key? key}) : super(key: key);
        
          @override
          Widget build(BuildContext context) {
            return MaterialApp(
              title: "Aplikasi Flutter Pertama",
              home: ProdukForm(),
            );
          }
        }
      
F. Produk Detail

- produk_detail.dart [Lihat File](aplikasi_flutter_pertamaku/lib/ui/produk_detail.dart
)<br>

main.dart untuk Produk Detail

        import 'package:flutter/material.dart';
        
        void main() {
          runApp(const MyApp());
        }
        
        class MyApp extends StatelessWidget {
          const MyApp({Key? key}) : super(key: key);
        
          @override
          Widget build(BuildContext context) {
            return MaterialApp(
              title: "Aplikasi Flutter Pertama",
              home: ProdukDetail(),
            );
          }
        }

### Membuat fungsi tombol simpan dan menampilkan data pada Detail Produk
- Buka kembali file produk_form.dart tambahkan attribute

      final _kodeProdukTextboxController = TextEditingController(); 
      final _namaProdukTextboxController = TextEditingController(); 
      final _hargaProdukTextboxController = TextEditingController();

- Pada setiap masing-masing TextField yang telah dibuat, data yang diinput dikirim ke attribute TextEditingController() yang telah kita buat sebelumnya

Pada fungsi _textboxKodeProduk() menjadi

          _textboxKodeProduk() { 
          return TextField( 
           decoration: const InputDecoration(labelText: "Kode Produk"), 
           controller: _kodeProdukTextboxController, 
           ); 
          }

Pada fungsi _textboxNamaProduk() menjadi

        _textboxNamaProduk() { 
        return TextField( 
         decoration: const InputDecoration(labelText: "Kode Produk"), 
         controller: _namaProdukTextboxController, 
         ); 
        }  

Pada fungsi _textboxhargaProduk() menjadi
   
        _textboxHargaProduk() { 
        return TextField( 
         decoration: const InputDecoration(labelText: "Kode Produk"), 
         controller: _hargaProdukTextboxController, 
         ); 
        }

Kemudian pada fungsi _tombolSimpan() pada saat diklik akan mengirim data inputan dan menampilkan data tersebut pada ProdukDetail yang telah kita buat sebelumnya

        _tombolSimpan() {
         return ElevatedButton(
         onPressed: () {
         String kodeProduk = _kodeProdukTextboxController.text;
         String namaProduk = _namaProdukTextboxController.text;
         int harga = int.parse(
         _hargaProdukTextboxController.text); //parsing dari String ke int
         // pindah ke halaman Produk Detail dan mengirim data
         Navigator.of(context).push(MaterialPageRoute(
         builder: (context) => ProdukDetail(
         kodeProduk: kodeProduk,
        61
         namaProduk: namaProduk,
        harga: harga,
         )));
         },
         child: const Text('Simpan'));
         }

G. Produk Page

- produk_page.dart [Lihat File](aplikasi_flutter_pertamaku/lib/ui/produk_page.dart)<br>

main.dart untuk Produk Page

        import 'package:aplikasi_flutter_pertamaku/ui/produk_page.dart';
        import 'package:flutter/material.dart';
                
        void main() {
          runApp(const MyApp());
        }
        
        class MyApp extends StatelessWidget {
          const MyApp({Key? key}) : super(key: key);
        
          @override
          Widget build(BuildContext context) {
            return MaterialApp(
              title: "Aplikasi Flutter Pertama",
              home: ProdukPage(),
            );
          }
        }


# Sekian Terima Kasih
