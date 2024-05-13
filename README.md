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

a. Hello World

- helloworld.dart [Lihat File](aplikasi)<br>

Didalamnya berisi code java, untuk menjalankan fungsi splash launcher. Lebih jelasnya splash launcher ini adalah menampilkan gambar/logo/icon ketika kita pertama kali membuka aplikasi, atau sebelum menuju kehalaman utama.

- backgroundlauncher.xml [Lihat File](tugasuasmobile/app/src/main/res/drawable/backgroundlauncher.xml)<br>

Ini adalah logo yang saya gunakan, saya menggunakan logo dari android studio nya

b. Source Code Utama

- MainActivity.java [Lihat File](tugasuasmobile/app/src/main/java/com/example/tugassepuluh/MainActivity.java)<br>

Di MainActivity ini berisi program java yang memiliki fungsi penghubung dari semua activity yang disebut intent dan fungsi tombol open alarm dan open map. Saya beri nama file ini Main karena disinilah fungsi paling awal dari halaman awal.

- activity_main.xml [Lihat File](tugasuasmobile/app/src/main/res/layout/activity_main.xml)<br>

Ini adalah layout dari halaman awal aplikasi ini. Layout ini terhubung dengan MainActivity.java tadi. Dilayout ini menampilkan semua tombol tombol dari berbagai activity dan program yang sudah dijelaskan diatas. Beginilah tampilan dari layoutnya :

![Screenshot_2024-01-15-08-32-56-735_com example tugassepuluh](https://github.com/amandaaaapn/ProjectUASMobile/assets/115678845/afbc1a9a-b07a-46ce-b16e-fc870f7224c9)

> Iconnya disini sudah Saya usahakan agar sesuai dengan identitas dari activitynya.

- AndroidManifest.xml [Lihat File](tugasuaasmobile/app/src/main/AndroidManifest.xml)<br>

Di AndroidManifest.xml ini berfungsi untuk mengaktifkan permission yang dibutuhkan dibeberapa activity. Selain itu, AndroidManifest.xml ini juga harus dilakukan pengeditan jika kita menambah sebuah tombol atau activity baru yang berhubungan dengan intent, agar activity tersebut dapat dibuka nantinya.

- string.xml [Lihat File](tugasuasmobile/app/src/main/res/values/strings.xml)<br>

String.xml ini adalah sebuah values, values ini berisi teks-teks dari tombol - isi - atau apapun itu yang berhubungan dengan teks.

- color.xml [Lihat File](tugasuasmobile/app/src/main/res/values/colors.xml)<br>

Sama seperti string, colors.xml ini juga merupakan sebuah values, tapi bedanya values ini berisi code-code warna yang sudah dibuat menjadi ID atau identitas yang bertujuan untuk memudahkan dalam pemanggilan warnanya di dalam coding.

c. Source Code Activity Hello World

- HelloActivity.java [Lihat File](tugasuasmobile/app/src/main/java/com/example/tugassepuluh/HelloActivity.java)<br>

Disini saya tidak mengubah apapun isi dari javanya, dengan kata lain saya buat default dari awal dibuat.

- activity_hello.xml [Lihat File](tugasuasmobile/app/src/main/res/layout/activity_hello.xml)<br>

Seperti yang sudah diketahui ini merupakan layout yang terhubung dengan java nya. Saya hanya menambahkan textview untuk menampilkan android:text "hello_world" nya (text sudah ada di string.xml), selain itu saya juga mengubah warna text dan menambahkan background agar terlihat lebih menarik.

- Hasil Run Hello World

![Screenshot_2024-01-15-08-33-06-287_com example tugassepuluh](https://github.com/amandaaaapn/ProjectUASMobile/assets/115678845/03fc1afd-a567-4ae7-a38f-c4fb369a08e4)

d. Source Code Activity Count

- CountActivity.java [Lihat File](tugasuasmobile/app/src/main/java/com/example/tugassepuluh/CountActivity.java)<br>

Tentunya disini berisi code java untuk menjalankan fungsi perhitungan dari rumus fibonnaci. Bilangan fibonnaci adalah bilangan yang rumusnya adalah menambah sebuah bilangan dengan bilangan sebelumnya. Contohnya 1, 1, 2, 3, 5, 8... 

- activity_count.xml [Lihat File](tugasuasmobile/app/src/main/res/layout/activity_count.xml)<br>

Ini adalah layout dari activity count, ada beberapa tombol disini seperti set limit, count, dan reset. Angka yang ditampilkan juga sudah menggunakan code warna, agar setiap angka yang ditampilkan memiliki warna yang berbeda dengan angka sebelumnya.

- Hasil Run Count

https://github.com/amandaaaapn/ProjectUASMobile/assets/115678845/9f51e69f-c208-44bc-bbab-204e90ceb4b1

e. Source Code Activity Scroll Movie

- SianidaActivity.java [Lihat File](tugasuasmobile/app/src/main/java/com/example/tugassepuluh/SianidaActivity.java)<br>

Disini saya tidak mengubah apapun isi dari javanya, dengan kata lain saya buat default sedari awal dibuat.

- activity_sianida.xml [Lihat File](tugasuasmobile/app/src/main/res/layout/activity_sianida.xml)<br>

Layout inilah yang mempengaruhi dan memberikan alasan kenapa di javanya tidak ada perubahan. Disini, digunakan sebuah scrollview yang bisa menjadikan text yang begitu panjang dan tidak muat dalam satu layar penuh, maka dengan ini kita bisa membaca semua isi kontennya hanya dengan cara scroll layar.

- Hasil Run Sianida

https://github.com/amandaaaapn/ProjectUASMobile/assets/115678845/52b4da88-9950-4fe8-b7c2-b6ec2a8ebb9d

f. Source Code Activity TwoActivity

- TwoActivity.java & TwoAct2Activity.java
  - TwoActActivity.java [Lihat File](tugasuasmobile/app/src/main/java/com/example/tugassepuluh/TwoactActivity.java) & TwoAct2Activity.java [Lihat File](tugasuasmobile/app/src/main/java/com/example/tugassepuluh/Twoact2Activity.java)<br>


Kedua java berisi fungsi untuk menjalankan program perpesanan. Kedua java tersebut memiliki peran masing-masing, yang pertama untuk pengirim dan yang kedua untuk fungsi ketika pesan berhasil terkirim.

- activity_twoact.xml & activity_twoact2.xml

  - activity_twoact [Lihat File](tugasuasmobile/app/src/main/res/layout/activity_twoact.xml) & activity_twoact2 [Lihat File](tugasuasmobile/app/src/main/res/layout/activity_twoact2.xml)<br>

Kedua layout ini merupakan tampilannya, yang pertama berfungsi menampilkan saat mengirim pesan dan yang kedua menampilkan saat pesan berhasil terkirim.

- Hasil Run TwoActivity

https://github.com/amandaaaapn/ProjectUASMobile/assets/115678845/1985db9f-e32a-4cfa-8666-1cc07b9f7673

g. Source Code Alarm

- Karena program ini hanya merupakan tombol, maka hanya tinggal menambahkan baris code berikut:

        # Tambahkan code ini didalam protected void OnCreate :
              findViewById(R.id.btnSetAlarm).setOnClickListener(v -> {
                  // Panggil metode untuk mengatur alarm
                  setAlarm();
              });
          }
        
        # Lalu code tambahkan fungsi intent untuk tombolnya :
          private void setAlarm() {
              Intent alarm = new Intent(AlarmClock.ACTION_SET_ALARM);
              startActivity(alarm);
          }

- Tidak hanya itu, perlu ditambahkan juga beberapa baris code di AndroidManifest.xml, seperti 
ini: 

          <uses-permission
                android:name="com.android.alarm.permission.SET_ALARM" />
          
          dan
              <action android:name="android.intent.action.SET_ALARM" />
  
- Hasil Run Alarm

https://github.com/amandaaaapn/ProjectUASMobile/assets/115678845/3376fc3f-b727-4327-b8c8-df55179210b6


h. Source Code Open Map

- Sama halnya seperti program alarm yang hanya menggunakan fungsi sebuah tombol, maka hanya code inilah yang diperlukan untuk dapat menjalankan dan membuka maps nya.

      # Tambahkan code ini didalam protected void OnCreate :
      ImageButton btnshowMap = findViewById(R.id.btnshowMap);
          btnshowMap.setOnClickListener(v -> {
              Intent map = new Intent(Intent.ACTION_VIEW, Uri.parse("geo:-6.324307,107.169273"));
              map.setPackage("com.google.android.apps.maps");
              startActivity(map);
          });

- Hasil Run Open Map

https://github.com/amandaaaapn/ProjectUASMobile/assets/115678845/05ba6b32-3a26-4afa-b7f2-49ec2e1051bb

i. Source Code Activity Fragment

Berbeda dari activity sebelumnya, di activity ini memerlukan banyak java dan layout, karena activity ini terdiri dari beberapa halaman. Perintah tugas dari activity ini adalah, membuat sebuah program atau aplikasi menampilkan daftar film sesuai dengan genre nya. Dan genre yang diperintahkan untuk dibuat ada tiga buah, yakni Action, Comedy, dan Romance.

- FragmentActivity.java [Lihat File](tugasuasmobile/app/src/main/java/com/example/tugassepuluh/FragmentActivity.java)<br>

Java yang ini berfungsi sebagai fungsi dari halaman utamanya. Didalamnya terdapat code untuk switch atau berpindah antar fragment dari action/comedy/romance. Nah agar code fragment tersebut dapat berjalan, perlu ditambahkan sebuah depedencies baru di build.gradlenya, berikut dependenciesnya :

      implementation("androidx.fragment:fragment:$fragmentVersion")

> Perlu diingat jika menambahkan dependencies baru, perlu dilakukan sync terlebih dahulu.

- activity_fragment.xml [Lihat File](tugasuasmobile/app/src/main/res/layout/activity_fragment.xml)<br>

Inilah layout yang terhubung dengan FragmentActivity.java, layout ini adalah tampilan basic atau tampilan utama yang masih kosong, didalamnya terdapat 3 tombol untuk berpindah antar fragment nya.

- FirstFragment.java [Lihat File](tugasuasmobile/app/src/main/res/layout/fragment_first.xml) , SecondFragment.java [Lihat File](tugasuasmobile/app/src/main/res/layout/fragment_second.xml) , ThirdFragment.java [Lihat File](tugasuasmobile/app/src/main/res/layout/fragment_third.xml) <br>

Nah ketiga java ini didalamnya terdapat fungsi untuk menampilkan list film yang ada, dan fungsi memutar trailer video ketika poster atau gambar filmnya ditekan. Video tersebut berasal dari link youtube yang saya tambahkan sesuai dengan film apa yang ada di masing masing fragment nya. Untuk menggunakan fungsi ini perlu ditambahkan depedencies di build.gradle nya. Saya menggunakan library yang bernama youtube player dari pierfrancescosoffritti, berikut dependenciesnya :

      implementation("com.pierfrancescosoffritti.androidyoutubeplayer:core:11.0.1")

> Perlu diingat jika menambahkan dependencies baru, perlu dilakukan sync terlebih dahulu.

- fragment_first.xml [Lihat File](tugasuasmobile/app/src/main/res/layout/fragment_first.xml) , fragment_second.xml  [Lihat File](tugasuasmobile/app/src/main/res/layout/fragment_second.xml) , fragment_third.xml [Lihat File](tugasuasmobile/app/src/main/res/layout/fragment_third.xml) <br>

Ketiga xml ini merupakan layout atau tampilan dari masing-masing fragment, didalamnya menampilkan daftar film sesuai dengan genrenya. Layout ini terhubung dengan ketiga java diatas.

- Hasil Run Fragment

https://github.com/amandaaaapn/ProjectUASMobile/assets/115678845/ff9f513d-4e64-4276-ba13-93ea4478a334

# Hasil Akhir dari semua Activity

https://github.com/amandaaaapn/ProjectUASMobile/assets/115678845/e182c84d-6b32-4fef-8d4e-7a960b47bec7

# Sekian Terima Kasih
