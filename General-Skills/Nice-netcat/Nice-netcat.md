## Challenge Name: Nice netcat...
Author: SYREAL
Category: General Skills
Tags: General Skills
Points: 15 points
Solve Rate: 96%

There is a nice program that you can talk to by using this command in a shell: $ nc mercury.picoctf.net 43239, but it doesn't speak English...

### Hints
1. You can practice using netcat with this picoGym problem: [what's a netcat?](https://play.picoctf.org/practice/challenge/34)
2. You can practice reading and writing ASCII with this picoGym problem: [Let's Warm Up](https://play.picoctf.org/practice/challenge/22)

### Approach
Open the picoCTF webshell at the side of your screen.
Login and type nc mercury.picoctf.net 43239 into the webshell.
We will get a bunch of random numbers, which is clearly in ASCII:
![image1](Nice-netcat_files/image1.png?raw=true "image1")
Simply paste it into any ASCII decoder, such as [CodeBeautify](https://codebeautify.org/ascii-to-text).
We can see the flag from there:
![image2](Nice-netcat_files/image2.png?raw=true "image2")

### Flag
picoCTF{g00d_k1tty!_n1c3_k1tty!_7c0821f5}

---
[Back to home](https://github.com/yanganyi/writeup-picogym)