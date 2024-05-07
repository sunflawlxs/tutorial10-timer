# Tutorial10 timer
Nama: Sheryl Ivana Widjaja<br>
NPM:2206824943<br>
Kelas: Advprog A <br>

## Refleksi 1

##### 1.2 Understanding how it works. 
![](images/images1.png)


Fungsi async bekerja secara independen dari fungsi utama yang memanggilnya. Ini berarti bahwa pelaksanaan fungsi async tidak bergantung pada pelaksanaan fungsi utama yang memanggilnya. Karena sifat asinkronusnya, urutan output dari program bisa berubah. Ada kemungkinan bahwa kode di luar fungsi async dieksekusi sebelum fungsi async selesai, yang menyebabkan perubahan urutan output yang diharapkan.

Saat menjalankan `cargo run`, ada kemungkinan "hey hey" muncul sebelum "howdy!" dan "done!". Hal ini disebabkan oleh fakta bahwa pernyataan `println!("hey hey");` berada di luar fungsi *async*, sehingga dapat dieksekusi secara independen dari eksekusi fungsi *async*.
