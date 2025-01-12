---
layout: post
title: Understanding how stacks Pop() works
date: 05-11-2024
categories: [Tugas-tugas]
tag: [Like, Comment]
image:
  path: /assets/images/foto1.jpg
---
# About
Memahami cara Stacks pop() bekerja adalah dengan cara melihat bagaimana data "ditumpuk" contoh dibawah ini jika kita memasukkan data 4 1 2 3 maka yang terjadi adalah seperti dibawah 
```
|3|
|2|
|1|
|4|
```
# Programnya
```python
stack = []

def push(stack, *elements): #*element untuk menaruh/push semua variable ke variable. element menjadi element = 1 2 3 4
    stack.extend(elements) #stack.extend (elements) di gunakan untuk menaruh apa yang ada di dalam element ke stack sekaligus

push(stack, 1, 2, 3, 4)
print (stack)

print([stack.pop() for i in range(len(stack))])
```