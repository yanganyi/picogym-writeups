## Challenge Name: Python Wrangling
Author: SYREAL
Category: General Skills
Tags: General Skills
Points: 10 points
Solve Rate: 93%

Python scripts are invoked kind of like programs in the Terminal... Can you run [this Python script](Python-Wrangling_files/ende.py) using [this password](Python-Wrangling_files/pw.txt) to get [the flag](Python-Wrangling_files/flag.txt.en)?

### Hints
1. Get the Python script accessible in your shell by entering the following command in the Terminal prompt: $ wget https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/ende.py
2. $ man python

### Approach
Get both the [Python script](Python-Wrangling_files/ende.py) and the [encrypted flag](Python-Wrangling_files/flag.txt.en) into the webshell using the following commands:
  $ wget https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/ende.py
  $ wget https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/flag.txt.en 
You should see something like this:
![image1](Python-Wrangling_files/image1.png?raw=true "image1")
Try:
  $ python3 ende.py
We see it gives the proper usage:
![image2](Python-Wrangling_files/image2.png?raw=true "image2")
Since -d stands for decode, try:
  $ python3 ende.py -d flag.txt.en
When it prompts you for the password, enter the password from the [file](Python-Wrangling_files/pw.txt).
You should be able to see the flag:
![image3](Python-Wrangling_files/image3.png?raw=true "image3")

### Flag
picoCTF{4p0110_1n_7h3_h0us3_aa821c16}

---
[Back to home](https://github.com/yanganyi/writeup-picogym)