---
layout: post
title: Nila Minimum Mahasiswa
date: 24-10-2024
categories: [Tugas-tugas]
tag: [Like, Comment]
image:
  path: /assets/images/foto5.jpg
---
# About
Program untuk menentukan kelulusan mahasiswa dari nilai. jika Angka yang dimasukkan lebih dari 100++ atau kurang dari 0-- maka program akan mengatakan "invalid value" 
# Program Python
```python
#user/player/entity memasukkan value nilai
value = int(input("Enter a value (0-100): "))

#if untuk memberitahu komputer bahwa barisan ini akan ada kondisi dan jika kondisi terpenuhi maka akan terprint "invalid value"
if value < 0 or value > 100:
    print("Invalid Value")
#elif dipakai jika if bagian atas sudah di pakai (di bagian ini digunakan untuk mengecek apakah nilai sama atau lebih tinggi dari 75)
elif value >= 75:
    print("Pass")
#else dipakai jika kondisi tidak memenuhi elif di atas atau if jika if yang di atas
else:
    print("Fail")
```
