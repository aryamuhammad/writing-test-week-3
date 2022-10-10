## Writing Test Week 3

### Array
- Definisi
 Array adalah tipe data yang dapat menampung berbagai tipe data apapun di dalamnya. Array memiliki 'sifat' list order yang dimulai dari index 0
![](asset/array.png)
- Array properties
  - .length 
    .length digunakan untuk mengetahui panjang dari suatu array
![](asset/array-length.png)
- Array Methods
  - push()
    Digunakan untuk menambahkan elemen baru ke akhir array
    ![](asset/push.png)
  - unshift()
    Digunakan untuk menambahkan elemen baru ke awal array
    ![](asset/unshift.png)
  - pop()
    Digunakan untuk menghapus elemen terakhir dari sebuah array
    ![](asset/pop.png)
  - shift() 
    Digunakan untuk menghapus elemen pertama dari sebuah array 
    ![](asset/shift.png)
  - splice()
    Digunakan untuk mengubah elemen yang ada di dalam array dengan menghapus, mengganti atau menambahkan elemen
    ![](asset/splice1.png)
    Penjelasan   
    - 2 merupakan index mulai untuk mengubah array
    - 1 merupakan berapa banyak elemen yang akan kita hapus
    ![](asset/splice2.png)
  - slice()  
    mengembalikan 'shallow copy' dari array tanpa mengubah struktur arraynya
    ![](asset/slice.png)
- Array Looping
    - for
    ![](asset/for%20loop.png)
    - for of
    ![](asset/for%20of.png)
    - forEach
    ![](asset/foreach.png)
    - map
    ![](asset/map.png)
- Array Multidimensi
Array yang berisikan Array
![](asset/arrmulti.png)
### Object
- Definisi
  Object adalah tipe data yang menyimpan property dan method 
- Membuat object
![](asset/object.png)
Penjelasan :
    - "nama" merupakan key dari object
    - "Arya" merupakan value dari key tersebut
- mengakses object
Terdapat beberapa cara dalam mengakses object
    - 1. dot notation
        ![](asset/dotnotation.png)
    - 2. bracket
       ![](asset/bracket.png) 
- membuat key
  membuat key baru dalam sebuah object:
  ![](asset/createkey.png)
- Assign object
  Menambahkan atau merubah key object
  ![](asset/assign.png)
- delete object
  Untuk mendelete key dari sebuah object, dapat menggunakan 'delete'
  ![](asset/delete.png)
- method object
  Method Object adalah function yang berada di dalam object
![](asset/method.png)
- nested object
  Nested object merupakan object bercabang atau object yang berada di dalam object
  ![](asset/nested.png)
- loop object
  Melakukan perulangan untuk setiap key yang ada di dalam object
  ![](asset/loop-obj.png)
  Key merujuk pada key yang ada di dalam object
- array of object
    Sebuah array yang menyimpan banyak object sebagai elemennya
    ![](asset/arrayofobject.png)
### Modules
- Definisi
  Javascript Modules adalah cara untuk memisahkan code ke file yang berbeda. Sehingga file file dapat terhubung antara satu dengan yang lainnya. Tujuannya agar code yang kita buat lebih mudah untuk dikelola   
  kita dapat melakukan export pada variabel, function, class
- Export
  Digunakan untuk mengekspor codingan untuk digunakan di file lain
  ![](asset/export.png)
- Import
  Digunakan untuk menangkap export
  ![](asset/import.png)
- Export Function 
  Melakukan export sebuah function agar function tersebut dapat digunakan/diakses pada file lain
  ![](asset/exportfunction.png)
  Setelah itu, kita import
  ![](asset/importfunction.png)
### Recursive
- Definisi 
  Recursive adalah function yang memanggil dirinya sendiri sampai suatu kondisi tertentu. Dalam menuliskannya kita dapat menambahkan type="module" pada script kita
- Base Case
  kondisi berhenti / kondisi paling kecil
- Recursion Case
  Kondisi dimana function tersebut memanggil function diri dia sendiri
- Contoh Recursive
  ![](asset/recursive.png)
  Penjelasan:
  Ketika kita memasukkan argumen 2 pada fungsi deret angka, kita cek dahulu apakah 3 == 1 ?
  ![](asset/exp1.png)
  Tentu bukan, maka dari itu masuk ke else 
  ![](asset/exp2.png)
  Setelah itu, function memanggil dirinya sendiri yang mana 3-1. maka n == 2. lalu diulang lagi proses seperti diatas. 
  ![](asset/exp1.png)
  apakah 2==1? false.   
  maka masuk ke else lagi
  ![](asset/exp2.png)
  Maka masuk ke function diri dia sendiri lagi, yang mana n-1 => 2-1 == 1 
  setelah itu, dicek lagi
  ![](asset/exp1.png)
  apakah n == 1? true.
  maka console.log(n) 
  maka tampil 1       
  Proses tersebut diulang ulang sampai function selesai.
### Asynchronous
- Ketika kita menuliskan baris code, baris code tersebut dibaca dari atas ke bawah. Ketika proses dari suatu baris code belum selesai, maka terjadi antrian.
  ![](asset/async.png)
- Javascript memiliki fitur Single Thread, Non-Blocking, dan Asynchronous
    - Single thread
        Hanya memiliki 1 jalur proses. yang mana saling tunggu menunggu sampai suatu proses selesai baru dapat menjalankan proses lain
    - Non-Blocking
        Mempersilahkan proses lain untuk dikerjakan apabila suatu proses membutuhkan waktu dalam mengerjakannya
    - Asynchronous
        Proses dapat didahului dan tidak harus dilakukan secara berurutan
- Callback
  Callback adalah function yang dijadikan argumen
- setTimeout()
  ![](asset/settimeout.png)
- Promise
  Promise simpelnya kita artikan sebagai janji. Promise mewakili penyelesaian atau kegagalan dari operasi asynchronus. Promise memiliki beberapa istilah:
    - Pending
        Kondisi awal dimana proses promise berjalan
    - Rejected
        Kondisi dimana promise gagal/ditolak
    - Fulfilled
        Kondisi dimana promise terpenuhi
  Cara membuat promise
  ![](asset/newPromise.png)
  Cara menangkap promise
  ![](asset/promisesexc.png)
### Web Storage
- Definisi
  Web Storage adalah storage yang dimiliki oleh web browser yang dapat menyimpan data di browser user
- Local Storage
  Menyimpan data tanpa expired date
- Session Storagae
  Menyimpan data dalam satu sesi (ketika browser tab ditutup, maka datanya hilang)
- Menyimpan ke local storage
  ![](asset/setitem.png)
- Mengakses ke local storage
  ![](asset/getitem.png)