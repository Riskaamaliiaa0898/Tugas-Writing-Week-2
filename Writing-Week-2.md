# Writing Minggu Ke-2

## JavaScript - Introduction
> JavaScript adalah bahasa pemograman yang sangat populer yang mudah digunakan.

> Syntax dan Statement (kamus pemograman) Contoh Syntax/ fungsi antara lain __Alert(), Prompt(), Confirm()__.

### Console.log
>__Console.log__ adalah perintah untuk mengecek dan mengetahui error pada code Pemograman web.

### Comments
>__Comments__ adalah .Comments tidak akan dijalankan oleh program karena hanya untuk dibaca oleh sesama programmer ataupun diri sendiri. 

Comment yang ada di JavaScript (JS)

    1. // ISI COMMENT => single Comment
    2. /*
        ini comment   => Multiline Comments
       */


Ada 6 tipe data fundamental pada Javascript
- number = tipe data yang mengandung semua angka termasuk angka desimal
    - semua angka 
    - Decimal 0,1 , 0,2 dll
- string = Grub Karakter dan harus diawali dan diakhiri dengan __single quotes ‘ … ‘__ ataupun __double quotes “ … “__.
- boolean = tipe data yang hanya mempunyai 2 buah nilai yaitu __TRUE (benar) or FALSE (salah)__.
- null = type data tidak memiliki nilai.
- undefined = tipe data yang merepresentasikan varibel/data yang tidak memiliki nilai.
- object = type data yang berhubungan dan dapat menyimpan data dengan tipe data apapun (number, string, boolean, dan lainnya).

### Variable 

>__Variable__ adalah container/tempat untuk menyimpan sebuah nilai

Ada 3 cara mendefinisikan sebuah variabel.
- cont = mutlak dan tidak bisa diubah
- var = pendevisian JS jadul
- let = pendevinisian JS yang sekarang

### Operator
1. Assignment operator (=) digunakan untuk menyimpan sebuah nilai pada variabel.
2. == adalah memjelaskan bentuk jenis sama misalkan 1 + '1' = 1
3. === adalah menjelaskan type yang sama atau berbeda. Misalkan 
1 + '1' = tidak ada jawaban

 Mathematical Assignment Operator

    Let W = 4;
    W = W+1;
    Console.log(W); // Output 5

> Arithmetic operator adalah operator yang melibatkan operasi matematika.
- Tambah (+)
- Kurang (-)
- Perkalian (*)
- Pembagian (/)
- Modulus (%) adalah sisa bagi 

### Comparision Operator

>__Comparition Operator__ Operator yang membandingkan satu nilai dengan nilai lainnya dan Hasil operasi yang melibatkan comparison operator adalah antara true or false.

Simbol comparison operator
- Lebih kecil dari : <
- Lebih besar dari: >
- Lebih kecil atau sama dengan: <=
- Lebih besar atau sama dengan: >=
- Sama dengan: ===
- Tidak sama dengan: !==

### Logical Operator
>__Logical operator__ biasa digunakan untuk sebuah CONDITIONAL pada pemograman.Menghasilkan nilai BOOLEAN yaitu TRUE or FALSE

Simbol dari Logical Operator adalah sebagai berikut:
- AND operator : && => AND akan menghasilkan nilai true jika kedua atau semua premis bernilai TRUE. sebaliknya apabila ada false dan true akan menghasilkan false
- OR operator: || => OR akan menghasilkan nilai true jika salah satu premis mengandung nilai TRUE
- NOT operator: ! => NOT akan membalikkan sebuah nilai BOOLEAN. TRUE menjadi FALSE dan sebaliknya.

## JavaScript - CONDITIONAL

> __Conditional__ merupakan statement percabangan yang menggambarkan suatu kondisi. Mengecek kondisi spesifik dan menjalankan perintah berdasarkan kondisi tersebut.

### Contoh Conditional

__IF Statement__

    if (true) {
    console.log('Berkas ini akan dikirim melalui Email!')}  
    
    // hasilnya "Berkas ini akan dikirim melalui Email!"

    if (False) {
        console.log('Perintah ini tidak akan dijalankan')}

    contoh IF 
    let lapar = true; 
    if (lapar) {
       console.log (' Yuk Makan ')}



__IF … ELSE Statement__ => Else akan mengeksekusi sebuah statement/code jika suatu kondisi bernilai FALSE.

    Contoh IF ... ElSE 

    Let Lapar = False;
    if (lapar) {
      console.log ('yuk makan') 
    } Else {
      Console.log ('tidak makan')} 

    // Selama kondisinya harus memenuhi satu saja caranya seperti ini
    let lapar = false
    if (lapar){
    console.log("Saya Makan")}


    Note:
    Bahwa let lapar=false/salah maka stetment 'tidak makan' akan dimunculkan sedangkan stetment 'yuk makan' tidak ditampilkan.


__IF .. ELSE IF Statement__ => dapat kita gunakan jika kita mempunyai berbagai kondisi.

    Contoh IF .. ELSE IF Statement

    char nilai;
 
    cout << "Input Nilai Anda (A - C): ";
    cin >> nilai;
 
    if (nilai == 'A' ) {
    cout << "Pertahankan!" << endl;
    } else if (nilai == 'B' ) {
    cout << "Harus lebih baik lagi" << endl;
    } else if (nilai == 'C' ) {
    cout << "Perbanyak belajar" << endl;
    {
    cout << "Maaf, format nilai tidak sesuai" << endl;
    } return 0;}

__Truthy and Falsy__ => digunakan untuk mengecek apakah variabel telah terisi namun tidak mementingkan nilainya.

    Contoh :

    // Truthy and Falsy ||
    let username = ""
    let dataUsername = username || "Agus"
    console.log(dataUsername)

    // Truthy and Falsy !
    console.log ('30' === 30) => output False
    console.log ('30' !== 30) => output true karena terdapat tanda seru


__Truthy and Falsy Assignment__ => Analoginya adalah jika kita memiliki sebuah website dan meminta inputan username lalu menampilkannya. Jika usernamenya kosong kita bisa isi nilai tersebut.

__Switch Case Conditional__ => Gunakan switch case jika kondisi dan percabangan terlalu banyak

    Contoh :

    // Switch Case
    let menu = 10

    switch(menu) {
        case 1 : {
         console.log("Menu 1")
         break;
        }
        case 2 : {
         console.log("Menu 2")
         break;
        }
        case 3 : {
         console.log("Menu 3")
         break;
        }
        default : {
         console.log("Anda salah memasukan menu")
         break;
        }
    }

__Ternary Operator(sintaks Singkat)__ => short-syntax dari statement if … else.

    Contoh :

    // Ternary Operator 
    let isNowSale = true
    isNowSale ? console.log("Shopping") : console.log("Not Shopping")

## JavaScript - LOOPING

> __Looping__ adalah statement yang mengulang sebuah instruksi hingga kondisi terpenuhi atau jika kondisi stop/berhenti tercapai.

- Manual Looping
-    __FOR LOOP__ => merupakan instruksi pengulangan yang dapat kita berikan pada program yang kita kembangkan.Gunakan FOR LOOP jika kita tahu seberapa banyak nilai pasti untuk pengulangannya

    Contoh :
    /* Perulangan */

    // For
    let n = 100
    for(let i=0 ; i < n+1; i++ ){
        console.log(i)
-    __WHILE LOOP__ akan menjalankan instruksi pengulangan kondisi bernilai TRUE.Gunakan WHILE LOOP jika kita tidak mengetahui jumlah pasti pengulangan.

    Contoh :
    let angka = 1
    while (angka <= 10){
        console.log(angka); angka++;
    }
-    __DO WHILE__ ingin menjalankan pengulangan 1 kali sebelum dilakukan pengecekan kondisi

    Contoh :
    do{
        Console.log("Nyala Mesin!");
        bensin--;
    } while (bensin > 0)

- __Nested Loop__ Jika kita membuat looping didalam looping. Maka ini dinamakan Nested Loop.


## Javascript - Scope
> __Scope__ adalah konsep dalam flow data variabel. Terdapat dua jenis variabel scope yang ada di JavaScript yaitu Global Variable dan Local Variable. 

__Local Scope__ adalah Variabel lokal hanya dapat diakses dari dalam fungsi tersebut. 

__Global Scope__ Semua variabel yang dibuat di luar fungsi disebut variabel global JavaScript. 

## JAVASCRIPT - FUNCTION
> __Function__ adalah sebuah blok kode dalam sebuah grup untuk menyelesaikan 1 task/1 fitur.

Membuat Function

    function greeting(){
        retrun 'hello World';
    };

Memanggil Function

    greeting ()
    Console.log(greeting));

## Parameter dan Argumen

### Parameter Function

    Function Penambahan(a, b) {
        return a + b;
    }
### Argumen Function
    Function Penambahan(a, b) {
        return a + b;
    }
    console.log(Penambahan(5, 5)) // output 10 

Default Parameters
> __Default paramaters__ digunakan untuk memberikan nilai awal/default pada parameter function. Default parameters bisa digunakan jika kita ingin menjaga function agar tidak error saat dipanggil tanpa argumen


    Function biodata(name= 'stranger') {
        return 'Hello ' + name;
    }
    console.log(biodata('riska')); //outputnya "Hello riska" -->
    console.log(biodata()); //outputnya "Hello stranger"

Function Helper
> Kita bisa menggunakan function yang sudah dibuat pada function lain.

Arrow Function
> Arrow function adalah cara lain menuliskan function. Ini adalah fitur terbaru yang ada pada ES6 (Javascript Version)

Short Syntax Function

## JavaScript dan HTML DOM

Setelah modul ini, kalian akan tahu tentang...
1. Overview proses rendering di browser
2. DOM dan perannya terkait browser dan HTML
3. Cara memanipulasi element HTML melalui DOM
4. Komunikasi antara HTML dan JavaScript melalui event 

Section Selecting elements

    getElementById() – select an element by id.

    getElementsByName() – select elements by name.

    getElementsByTagName()  – select elements by a tag name.

    getElementsByClassName() – select elements by one or more class names.

    querySelector()  – select elements by CSS selectors.

Manipulating elements HTML

Caranya
Mencari Element HTML
Mengubah Konten Element (Element.textContent dapat kita gunakan untuk
mengubah teks di dalam sebuah element
)
- Element.textContent
    
        .textContent = “<span>Teks Heading</span”

- Element.innerHTML

        .innerHTML = “<span>Teks Heading</span”





