---
layout: post
title: Menemukan kata palindrome python
date: 26-10-2024
categories: [Tugas-tugas]
tag: [Like, Comment]
image:
  path: /assets/images/foto2.jpg
---

# About
Cara menemukan kata palindrome di python adalah dengan membalik kata itu dan membandingkan nya pada saat belum dibalik jika sama maka itu palindrome jika tidak maka bukan

# Programnya
```python
string ="kakak" #masukkan kata

def is_palindrome(string): #untuk mengecek apakah kalimat adalah palindrome
  if string == string[::-1]: #membalikkan string original dengan yang sudah di balik apakah sama atau tidak
    return True
  else:
    return False

if is_palindrome (string): #line ini untuk print berdasarkan hasil di atas
  print(string, "= palindrome.") #jika di atas hasil nya true maka print "= palindrome"
else:
  print(string, "= it aint palindrome.") #jika tidak maka print  = it aint palindrome"
  ```