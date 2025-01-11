---
layout: post
title: Temukan Nilai terkecil Menggunakan Stacks dalam program
date: 11-06-2024
categories: [Tugas-tugas]
tag: [Like, Comment]
image:
  path: /assets/lib/foto6.jpg
---

# About
Program untuk menemukan angka terkecil dari barisan angka [10 9 6] dengan cara membandingkan 1 persatu dan menggunakan pop() jika menemukan angka yang lebih kecil

# Programnya
```python
def push(stack, index):
    stack.append(index)

def pop(stack):
    if stack:
        return stack.pop()
    else:
        return None
    
def top(stack):
    if stack:
        return stack[-1]
    return None

stack = [int(x) for x in input("Angka (pisahkan dengan spasi): ").split()]
#split () untuk mengubah setiap inputan yang dipisahkan dari spasi menjadi string yang berbeda contoh "1 2 3" > "1", "2", "3"
# x = "1" > int(x) = 1
# x = "2" > int(x) = 2
# x = "3" > int(x) = 3
#maka nanti dibaca [1, 2, 3] oleh line dibawah 
kecil = []


while stack:
    index = pop(stack) #menaruh element terakhir di stack ke index dan juga menghapus
    while kecil and kecil[-1] < index: #jika semua angka yang didalam (kecil) lebih besar dari index
        push(stack, pop(kecil)) #maka semua angka yang lebih besar dari index itu akan kembali ke stack dan menghapus nya di kecil
    push(kecil, index) #menaruh angka yang ada di index ke (kecil)

print(top(kecil))
```