---
layout: post
title: Program Mendata Mahasiswa
date: 24-10-2024
categories: [Tugas-tugas]
tag: [Like, Comment]
image:
  path: /assets/lib/foto4.png
---
# About
Program yang ada di bawah ini untuk mendata mahasiswa dengan mencatat NIM, Jurusan dan Nama menggunakan python dan variable ksosong yang akan di isi oleh data
# Data Mahasiswa Python
```Program python nya```
```python
jumlah_mahasiswa = int(input("Masukkan jumlah mahasiswa:" )) #entitas memasukkan angka
empty = [] #variable kosong yang akan diisi saat looping

for angka in range(jumlah_mahasiswa): #tergantung seberapa banyak angka yang user input sebanyak itu pula looping berjalan
    nim = input(f"NIM Mahasiswa ke-{angka+1}: ") #untuk user menginput NIM mahasiswa dan akan di ulang tergantung seberapa banyak jumlah maha di input tadi
    nama = input (f"Nama Mahasiswa ke-{angka+1}: ") #{angka+1} supaya user tidak bingung ini mahasiswa yang ke berapa
    jurusan = input (f"Jurusan Mahasiswa ke-{angka+1}: ") #umm i honestly dont know what to explain but basiclly just like the above
    empty.append (nim) #setor informasi yang sudah di input sama user ke variables (empty) makanya namanya empty :>
    empty.append (nama) #setor informasi yang sudah di input sama user ke variables (empty) makanya namanya empty :>
    empty.append (jurusan) #setor informasi yang sudah di input sama user ke variables (empty) makanya namanya empty :>

print ("DATA MAHASISWA YANG DIMASUKKAN") #ummm kalo kata koh rei atau kak hendra biar rapi dan enak diliat outputnya
print ("------------------------------") #ummm kalo kata koh rei atau kak hendra biar rapi dan enak diliat outputnya
print ("NIM         NAMA       JURUSAN") #ummm kalo kata koh rei atau kak hendra biar rapi dan enak diliat outputnya

for i in range(0, len(empty), 3): #menghitung jumlah variable yang di dalam (empty) 
    nim, nama, jurusan = empty[i:i+3] #mempisah pisah data yang ada di (empty) supaya bisa di print
    print(f"{nim:<13} {nama:<13} {jurusan:<13}") #supaya selaras dengan NIM, NAMA, dan JURUSAN di atasnya ketika di output
```
