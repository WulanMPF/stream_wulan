# JOBSHEET 12 (PRAKTIKUM 1-5)

Nama: Wulan Maulidya P. F

Kelas: TI-3H

No. Absen: 27

NIM: 2241720174

---

## PRAKTIKUM 1

### Langkah 1: Buat Project Baru

Buatlah sebuah project flutter baru dengan nama stream_nama (beri nama panggilan Anda) di folder week-12/src/ repository GitHub Anda.

### Langkah 2: Buka file main.dart
Ketiklah kode seperti berikut ini.

![Praktikum](/images/p1_l2.png)

**Soal 1** Tambahkan nama panggilan Anda pada title app sebagai identitas hasil pekerjaan Anda. Gantilah warna tema aplikasi sesuai kesukaan Anda.

![Praktikum](/images/p1_l2a.png)

### Langkah 3: Buat file baru stream.dart
Buat file baru di folder lib project Anda. Lalu isi dengan kode berikut.

![Praktikum](/images/p1_l3.png)

### Langkah 4: Tambah variabel colors
Tambahkan variabel di dalam class ColorStream seperti berikut.

![Praktikum](/images/p1_l4.png)

**Soal 2** Tambahkan 5 warna lainnya sesuai keinginan Anda pada variabel colors tersebut.

![Praktikum](/images/p1_l4a.png)

### Langkah 5: Tambah method getColors()
Di dalam class ColorStream ketik method seperti kode berikut. Perhatikan tanda bintang di akhir keyword async* (ini digunakan untuk melakukan Stream data)

![Praktikum](/images/p1_l5.png)

### Langkah 6: Tambah perintah yield*
Tambahkan kode berikut ini.

![Praktikum](/images/p1_l6.png)

**Soal 3** Jelaskan fungsi keyword yield* pada kode tersebut! Apa maksud isi perintah kode tersebut?

* Keyword yield* dalam Dart digunakan dalam konteks generator function untuk meneruskan hasil dari satu generator (atau stream) ke generator lainnya. Dalam kode tersebut, yield* digunakan untuk mengalirkan nilai dari stream yang dihasilkan oleh Stream.periodic.
* Isi perintah kode tersebut bertujuan untuk menghasilkan stream warna secara berulang setiap detik. Setiap detik, kode akan mengembalikan satu warna dari daftar colors, lalu kembali ke awal daftar setelah mencapai akhir. Sehingga, stream akan menerima warna baru setiap detik sesuai dengan urutan yang ditentukan dalam daftar colors.

### Langkah 7: Buka main.dart
Ketik kode impor file ini pada file main.dart

![Praktikum](/images/p1_l7.png)

### Langkah 8: Tambah variabel
Ketik dua properti ini di dalam class _StreamHomePageState

![Praktikum](/images/p1_l8.png)

### Langkah 9: Tambah method changeColor()
Tetap di file main, Ketik kode seperti berikut

![Praktikum](/images/p1_l9.png)

### Langkah 10: Lakukan override initState()
Ketika kode seperti berikut

![Praktikum](/images/p1_l10.png)

### Langkah 11: Ubah isi Scaffold()
Sesuaikan kode seperti berikut.

![Praktikum](/images/p1_l11.png)

### Langkah 12: Run
Lakukan running pada aplikasi Flutter Anda, maka akan terlihat berubah warna background setiap detik.

![Praktikum](/images/p1_l12.gif)

**Soal 4** Capture hasil praktikum Anda berupa GIF dan lampirkan di README. Lakukan commit hasil jawaban Soal 4 dengan pesan "W12: Jawaban Soal 4"

### Langkah 13: Ganti isi method changeColor()
Anda boleh comment atau hapus kode sebelumnya, lalu ketika kode seperti berikut.

![Praktikum](/images/p1_l13.png)

**Soal 5** Jelaskan perbedaan menggunakan listen dan await for (langkah 9) !

* listen lebih fleksibel dan memungkinkan untuk tetap menjalankan kode lain sambil menunggu nilai dari stream.
* await for memberikan cara yang lebih terstruktur untuk menangani stream, tetapi menghambat eksekusi kode setelahnya sampai stream selesai.

## PRAKTIKUM 2

### Langkah 1: Buka file stream.dart
Lakukan impor dengan mengetik kode ini.

![Praktikum](/images/p2_l1.png)

### Langkah 2: Tambah class NumberStream
Tetap di file stream.dart tambah class baru seperti berikut.

![Praktikum](/images/p2_l2.png)

### Langkah 3: Tambah StreamController
Di dalam class NumberStream buatlah variabel seperti berikut.

![Praktikum](/images/p2_l3.png)

### Langkah 4: Tambah method addNumberToSink
Tetap di class NumberStream buatlah method ini

![Praktikum](/images/p2_l4.png)

### Langkah 5: Tambah method close()

![Praktikum](/images/p2_l5.png)

### Langkah 6: Buka main.dart
Ketik kode import seperti berikut

![Praktikum](/images/p2_l6.png)

### Langkah 7: Tambah variabel
Di dalam class _StreamHomePageState ketik variabel berikut

![Praktikum](/images/p2_l7.png)

### Langkah 8: Edit initState()

![Praktikum](/images/p2_l8.png)

### Langkah 9: Edit dispose()

![Praktikum](/images/p2_l9.png)

### Langkah 10: Tambah method addRandomNumber()

![Praktikum](/images/p2_l10.png)

### Langkah 11: Edit method build()

![Praktikum](/images/p2_l11.png)

### Langkah 12: Run
Lakukan running pada aplikasi Flutter Anda, maka akan terlihat seperti gambar berikut.

![Praktikum](/images/p2_l12.gif)

**Soal 6** Jelaskan maksud kode langkah 8 dan 10 tersebut!

* initState() menginisialisasi stream dan mendengarkan data yang masuk, memastikan UI diperbarui setiap kali ada angka baru.
* addRandomNumber() digunakan untuk menghasilkan angka acak dan menambahkannya ke stream, yang kemudian akan memicu pembaruan pada tampilan aplikasi.

### Langkah 13: Buka stream.dart
Tambahkan method berikut ini.

![Praktikum](/images/p2_l13.png)

### Langkah 14: Buka main.dart
Tambahkan method onError di dalam class StreamHomePageState pada method listen di fungsi initState() seperti berikut ini.

![Praktikum](/images/p2_l14.png)

### Langkah 15: Edit method addRandomNumber()
Lakukan comment pada dua baris kode berikut, lalu ketik kode seperti berikut ini.

![Praktikum](/images/p2_l15.png)

**Soal 7** Jelaskan maksud kode langkah 13 sampai 15 tersebut!. Kembalikan kode seperti semula pada Langkah 15, comment addError() agar Anda dapat melanjutkan ke praktikum 3 berikutnya.

* Langkah 13: Metode ini digunakan untuk menambahkan kesalahan ke dalam stream. Saat dipanggil, ia menggunakan sink dari controller untuk mengirimkan pesan kesalahan ('error').
* Langkah 14: Menerapkan penanganan kesalahan yang membuat aplikasi lebih robust dan responsif terhadap masalah yang mungkin terjadi saat menerima data.
* Langkah 15: Mengubah fungsionalitas dari menambahkan angka acak menjadi mensimulasikan kesalahan. Ini memungkinkan pengujian bagaimana aplikasi merespons ketika ada kesalahan, dan bagaimana UI diperbarui (misalnya, menampilkan -1 pada lastNumber).
* Mengembalikan kode seperti semula pada Langkah 15

![Praktikum](/images/p2_l15a.png)

![Praktikum](/images/p2_l15b.png)

## PRAKTIKUM 3

### Langkah 1: Buka main.dart
Tambahkan variabel baru di dalam class _StreamHomePageState

![Praktikum](/images/p3_l1.png)

### Langkah 2: Tambahkan kode ini di initState

![Praktikum](/images/p3_l2.png)

### Langkah 3: Tetap di initState
Lakukan edit seperti kode berikut.

![Praktikum](/images/p3_l3.png)

### Langkah 4: Run
Terakhir, run atau tekan F5 untuk melihat hasilnya jika memang belum running. Bisa juga lakukan hot restart jika aplikasi sudah running. Maka hasilnya akan seperti gambar berikut ini. Anda akan melihat tampilan angka dari 0 hingga 90.

![Praktikum](/images/p3_l4.gif)

**Soal 8** Jelaskan maksud kode langkah 1-3 tersebut!

* Langkah 1: Menambahkan variabel transformer bertipe StreamTransformer untuk memanipulasi data yang mengalir melalui stream.
* Langkah 2: Menginisialisasi transformer di metode initState, dengan fungsi untuk menggandakan nilai yang diterima, menangani kesalahan dengan mengirimkan -1, dan menutup aliran ketika selesai.
* Langkah 3: Menggunakan transformer untuk memproses stream, dengan mendengarkan nilai yang telah ditransformasikan dan memperbarui lastNumber di state. Juga, menambahkan penanganan kesalahan untuk mengatur lastNumber ke -1 jika terjadi kesalahan.

## PRAKTIKUM 4

### Langkah 1: Tambah variabel
Tambahkan variabel berikut di class _StreamHomePageState

![Praktikum](/images/p4_l1.png)

### Langkah 2: Edit initState()
Edit kode seperti berikut ini.

![Praktikum](/images/p4_l2.png)

### Langkah 3: Tetap di initState()
Tambahkan kode berikut ini.

![Praktikum](/images/p4_l3.png)

### Langkah 4: Tambah properti onDone()
Tambahkan dibawahnya kode ini setelah onError

![Praktikum](/images/p4_l4.png)

### Langkah 5: Tambah method baru
Ketik method ini di dalam class _StreamHomePageState

![Praktikum](/images/p4_l5.png)

### Langkah 6: Pindah ke method dispose()
Jika method dispose() belum ada, Anda dapat mengetiknya dan dibuat override. Ketik kode ini didalamnya.

![Praktikum](/images/p4_l6.png)

### Langkah 7: Pindah ke method build()
Tambahkan button kedua dengan isi kode seperti berikut ini.

![Praktikum](/images/p4_l7.png)

### Langkah 8: Edit method addRandomNumber()
Edit kode seperti berikut ini.

![Praktikum](/images/p4_l8.png)

### Langkah 9: Run
Anda akan melihat dua button seperti gambar berikut.

![Praktikum](/images/p4_l9.png)

### Langkah 10: Tekan button ‘Stop Subscription'
Anda akan melihat pesan di Debug Console seperti berikut.

![Praktikum](/images/p4_l10.gif)

**Soal 9** Jelaskan maksud kode langkah 2, 6 dan 8 tersebut!

* Langkah 2: Di dalam initState(), menginisialisasi numberStream dan numberStreamController, lalu mendengarkan stream untuk menangkap event. Dengan menggunakan subscription, maka menyimpan referensi ke listener, sehingga ketika data baru diterima, kita dapat memperbarui lastNumber dan merender UI.
* Langkah 6: Dalam metode dispose(), membatalkan subscription untuk menghentikan pendengar dari mendengarkan stream. Hal ini penting untuk membebaskan sumber daya dan mencegah kebocoran memori ketika widget dihapus dari pohon widget.
* Langkah 8: Di metode addRandomNumber(), menghasilkan angka acak dan memeriksa apakah numberStreamController masih terbuka. Jika terbuka, angka acak ditambahkan ke sink; jika tidak, lastNumber diatur ke -1 untuk menunjukkan bahwa penambahan angka gagal.

## PRAKTIKUM 5

### Langkah 1: Buka file main.dart
Ketik variabel berikut di class _StreamHomePageState

![Praktikum](/images/p5_l1.png)

### Langkah 2: Edit initState()
Ketik kode seperti berikut.

![Praktikum](/images/p5_l2.png)

### Langkah 3: Run
Lakukan run maka akan tampil error seperti gambar berikut.

![Praktikum](/images/p5_l3.png)

**Soal 10** Jelaskan mengapa error itu bisa terjadi ?

* Jika numberStreamController tidak diinisialisasi sebagai broadcast stream, maka stream tersebut hanya bisa didengarkan satu kali. Saat mencoba untuk melakukan listen pada stream yang sama lebih dari sekali, error ini muncul.
* Jika mencoba untuk menambahkan dua listener yang berbeda (subscription dan subscription2) pada stream yang sama. Jika stream tersebut bukan broadcast, ini menyebabkan error.
* Jika numberStreamController tidak dideklarasikan dengan StreamController.broadcast(), maka secara default akan menjadi StreamController biasa. Ini berarti hanya dapat mendengarkan stream tersebut satu kali. Upaya untuk mendengarkan kembali stream yang sama akan menyebabkan error.

### Langkah 4: Set broadcast stream
Ketik kode seperti berikut di method initState()

![Praktikum](/images/p5_l4.png)

### Langkah 5: Edit method build()
Tambahkan text seperti berikut

![Praktikum](/images/p5_l5.png)

### Langkah 6: Run
Tekan button ‘New Random Number' beberapa kali, maka akan tampil teks angka terus bertambah sebanyak dua kali.

![Praktikum](/images/p5_l6.gif)

**Soal 11** Jelaskan mengapa hal itu bisa terjadi ?

* Dengan mengubah stream menjadi broadcast, akan mengatasi error yang muncul saat mencoba menambahkan lebih dari satu listener. Kode tersebut dapat menampilkan teks angka yang terus bertambah karena kedua listener menerima dan memproses event yang sama, sehingga nilai yang ditambahkan ke values di-update dua kali setiap kali event baru diterima.
