# Tugas Modul Praktikum 3

## Latihan 1
Pada latihan 1 kali ini kita akan mencari angka terkecil yang kurang dari 0,5. Berikut algoritma dan langkah-langkahnya:
##### A. Input 
 - Langkah pertama, kita harus membuat perintah untuk memasukan nilai N 
```
num = int(input("Masukan nilai N: "))
```
 - Langkah kedua, kita akan membuat variable untuk menentukan berapa jumlah data yang ingin di cari.
```
jumlah = num+1
start = 1
stop = jumlah
step = 1
```
"start = 1" berarti data dimulai dari 1. "jumlah = r+1 dan stop = jumlah" berarti looping akan berhenti ketika variable 'jumlah' sudah sesuai dengan nilai yang diinput pada variable 'N'.
##### B. Process
 - Langkah ketiga, kita menggunakan syntax looping for, untuk memulai dan mengakhiri looping sesuai input start, stop dan step yang sudah kita masukan di langkah sebelumnya.
```
for i in range(start, stop, step):
```
 - Langkah keempat, masukan perintah sebagai berikut dengan menggunakan fungsi random:
```
from random import random
    a = random()
```
##### C. Output 
 - Terakhir masukan perintah 'print' untuk menampilkan hasil dari input variable.
```
print("Data ke:",i,"=>",(a))
```
'i' adalah hasil dari jumlah perulangan yang telah dilakukan. Dan 'a' akan menampilkan nilai secara acak karena fungsi random yang telah diinput.
### Gambar hasil latihan 1
![Latihan1](https://user-images.githubusercontent.com/56240386/72215875-e3ddba80-354b-11ea-9ed3-10dcb91f9988.png)


## Latihan 2
Pada latihan 2 kali ini kita akan menampilkan bilangan terbesar dari N buah data yang diinpukan, dan angka 0 digunakan untuk berhenti. Berikut algoritma dan langkah-langkahnya:
##### A. Input
 - Pertama membuat 2 variable, masukan variable 'a' sebagai integer, kemudian menginputkan nilainya. Dan variable 'b' dengan nilai 0.
```
a = int()
b = 0
```
##### B. Process
 - Kedua, menggunakan looping while. Disini kita akan diminta untuk menginput angka pada variable 'a'. Dan apabila nilai 'a' lebih besar dari 0, maka akan terjadi perulangan.
```
while a >= 0:
    a = int(input("Masukan Bilangan: "))
```
 - Ketiga, Membuat statement untuk mengambil angka terbesar. Disini system akan mengambil nilai 'a' terbesar untuk variable 'b'.
```
 if a > b:
        b = a
```
 - Keempat, Membuat statement untuk berhenti dari perulangan. Pada tahap ini apabila kita menginput nilai 0 pada variable 'a' yang diminta sebelumnya, maka kita akan berhenti dari perulangan.
```
 if a == 0:
       break
```
##### C. Output
 - Terakhir, gunakan perintah 'print' mencetak bilangan terbesar.
```
print("Bilangan terbesar adalah", b)
```
### Gambar hasil latihan 2
![Latihan2](https://user-images.githubusercontent.com/56240386/72215887-066fd380-354c-11ea-82a4-9e8eb3c3efa9.png)


## Program 1
Pada program 1 kali ini kita akan menghitung laba keuntungan per-bulan. Berikut algoritma dan langkah-langkahnya:
##### A. Input
 - Langkah pertama, kita membuat variable dengan nilai modal = 1000000000, nilai laba dan untung adalah 0.
```
modal = 1000000000
laba = 0                                  
untung = 0
```
##### B. Process 
 - Selanjutnya menggunakan perulangan for, Disini perulangan akan dimulai dari nilai 1 dan akan berhenti pada nilai akhir, yaitu 9.
```
for i in range (1,9):
```
 - Lalu, masukan kondisi 1 apabila belum bulan ke-3 laba masih 0%, kondisi 2 apabila belum memasuki bulan ke-5 mendapat laba sebesar 1%, kondisi 3 apabila belum memasuki bulan ke-8 mendapat laba 5%, dan pada bulan ke-8 laba menurun 2%, maka laba bulan ke-8 sebesar 3%.
```
    if (i < 3):                  ## "if" = bila suatu kodisi tertentu tercapai maka apa yang harus dilakukan dengan fungsi ini kita bisa menjalankan sesuatu
        laba = 0
        untung = untung + laba
    elif(i < 5):                 ## "elif" = adalah ketika kondisi lainnya tercapai maka jalankan program.
        laba = modal*1/100
        untung = untung + laba
    elif(i < 8):
        laba = modal*5/100
        untung = untung + laba
    else:                        ## "else" = adalah ketika tidak ada suatu kondisi yang terpenuhi maka jalankan program.
        laba = modal*2/100
        untung = untung + laba
```
##### C. Output 
 - Terakhir gunakan perintah 'print' untuk menampilkan hasil laba perbulan dan total laba selama 8 bulan.
```
    print("Laba bulan ke", i, "sebesar:", laba)
print("Total laba adalah : ", untung)
```
### Gambar hasil program 1
![Program1](https://user-images.githubusercontent.com/56240386/72215899-230c0b80-354c-11ea-81cf-2aad9f451f21.png)

