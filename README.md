# Belajar JavaScript

Ini adalah dokumen yang dipakai untuk video series [Belajar JavaScript](https://youtube.com/playlist?list=PLJqG5Qok4qr0ncLt-omRe6mt6tFsXTSXU) di channel YouTube ku.

## Daftar Isi

- [Belajar JavaScript](#belajar-javascript)
  - [Daftar Isi](#daftar-isi)
  - [Apa itu JavaScript](#apa-itu-javascript)
  - [Persiapan belajar](#persiapan-belajar)
  - [console.log](#consolelog)
  - [Memberikan komentar](#memberikan-komentar)
  - [Tipe data](#tipe-data)
    - [Number](#number)
    - [String](#string)
  - [Variables](#variables)
  - [Array](#array)
  - [Properties (Properti)](#properties-properti)
  - [Methods (Metode)](#methods-metode)

## Apa itu JavaScript

JavaScript adalah salah satu bahasa programming yang sangat populer. Demikian karena JavaScript adalah satu-satunya bahasa yang dapat membuat website lebih interaktif. Bukan cuma untuk website, bahasa ini juga sering digunakan untuk membangun server, aplikasi mobile, dan software.

Ketika kamu mengerjakan project yang lebih besar, otomatis kode yang kamu tulis akan lebih kompleks. Untuk mempermudah pengerjaan project, biasanya developer akan memilih TypeScript daripada JavaScript. Typescript adalah bahasa programming yang dimana syntax (cara penulisan) nya sama dengan JavaScript, tapi memiliki lebih banyak fitur untuk mempermudah proses pemrograman.

Ada kalanya kamu mendengar kata EcmaScript. EcmaScript (disingkatnya ES) adalah standarisasi untuk bahasa JavaScript. Gampangnya, JavaScript itu disusun berdasarkan aturan yang ada di EcmaScript. Dan EcmaScript itu berevolusi.

Mungkin ketika kamu membaca paragraf 2 dan 3 itu rada serem dan mengintimidasi... Tapi tenang aja, berikut garis bawahnya:

- JavaScript adalah bahasa programming yang biasa dipakai untuk membuat website lebih interaktif, membangun server, membangun software & aplikasi mobile
- Project yang lebih besar disarankan menggunakan TypeScript
- EcmaScript adalah standarisasi JavaScript

## Persiapan belajar

Selama proses pembelajaran, aku akan menggunakan [jsitor.com](https://jsitor.com/). Kamu boleh memilih environment lain seperti [Codepen](https://codepen.io/), atau menggunakan code editor dan menjalankan file nya di browser.

Kamu juga bebas memilih browser apa saja, pastikan kamu bisa membuka Developer Tools di browser tersebut.

## console.log

Aku mau kenalin kamu fungsi yang sangat sering dipakai ketika debugging*.

_Debugging adalah proses mencari dan menghapus bug atau error pada suatu program._

```js
console.log("belajar javascript");
```

Kode diatas akan memunculkan teks "belajar javascript" (tanpa tanda kutip) di console. Di jsitor, klik tombol console untuk melihat layar tersebut. Atau buka Developer Tools > Console.

Buat barisan baru, dan tambahkan kode berikut `console.log("js singkatan dari JavaScript");`. Kode keseluruhan akan menjadi seperti ini:

```js
console.log("belajar javascript");
console.log("js singkatan dari JavaScript");
```

Perhatikan layar console. Teks "belajar javascript" di keluarkan lebih dulu, baru setelah itu "js singkatan dari JavaScript". Artinya, kode dijalankan mulai dari yang paling atas kemudian yang bawah.

Lalu bagaimana kalau kode yang seperti ini:

```js
console.log("baris ke-1");console.log("samping");
console.log("baris ke-2");
```

Hasil yang ada di console adalah:

```txt
baris ke-1
samping
baris ke-2
```

Dari sini, kita bisa ambil kesimpulan bahwa kode akan berjalan mulai dari atas, kemudian kesamping, lalu kebawah.

Perlu diperhatikan, kalau setiap console.log diakhiri dengan titik koma (;).

Kita diperbolehkan untuk menghapus titik koma tersebut, seperti berikut:

```js
console.log("baris ke-1")
console.log("baris ke-2")
```

Namun kode berikut akan menghasilkan error:

```js
console.log("baris ke-1") console.log("samping")
console.log("baris ke-2")
```

Khusus instruksi yang seperti ini, kita tidak diperbolehkan untuk menulis instruksi di samping (baris yang sama). Namun tidak semua instruksi akan muncul error ketika ditulis menyamping seperti ini.

Ini akan lebih mudah dipahami ketika nanti kita lebih ngoding.

Untuk sekarang, kita tulis kodenya dari atas kebawah aja, daripada menyamping. Karena susunan atas ke bawah itu lebih gampang dibaca.

## Memberikan komentar

Comments (komentar) itu digunakan untuk menulis teks yang tidak akan dijalankan program. Teks ini biasanya untuk memberi kejelasan atau detail suatu kode.

Ada dua jenis komentar. Single-line comment:

```js
// Tulis apa aja disini...
```

Multi-line comment:

```js
/*
  Apa aja disini ditulis...
  tulis apa disini...
  disini aja tulis apa...
*/
```

## Tipe data

Setiap data ada jenisnya atau kita sebut tipe data.

- Number
- String
- Boolean
- undefined
- null
- Symbol
- Object

### Number

Sesuai namanya, number itu data yang berupa angka numerik. Bisa negatif, positif, dan desimal.

```js
console.log(1)
console.log(-1)
console.log(-1.34)
```

Kamu juga bisa melakukan operasi perhitungan. Simbol-simbol ini (-, +, dll.) sebutannya operator.

```js
console.log(1 + 1)
console.log(2 - 5)
console.log(3.2 * 10 / 2)
console.log(4.6 - (1 - 4))
```

### String

String adalah data yang berbentuk teks. Teks ini ditulis di antara tanda kutip.

```js
console.log('boleh begini')
console.log("yang ini boleh")
console.log(`begini boleh juga`)
```

single quote ('), double quote ("), backtick (`).

Hampir semua karakter bisa dimasukkan ke dalam string. Tapi ada beberapa karakter tidak bisa ditulis secara langsung, tetapi harus diawali garis miring terbalik atau backslash (\\).

<!-- misal lagi bikin pantun -->
```js
console.log('baris pertama\nbaris kedua')
console.log(`baris pertama
baris kedua`)

console.log(`harga ciki * 2 bngkus = ${4000 * 2}`)

```

Kita juga bisa menggabungkan antara 2 string atau lebih. Ini disebutnya String Concatenation.

```js
console.log('panas dalam')
console.log('panas' + 'dalam')
console.log('panas' + ' ' + 'dalam')
```

## Variables

## Array

## Properties (Properti)

## Methods (Metode)
