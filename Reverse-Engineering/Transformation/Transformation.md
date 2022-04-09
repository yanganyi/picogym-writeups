## Challenge Name: Transformation
Author: MADSTACKS
Category: Reverse Engineering
Tags: Reverse Engineering
Points: 20 points
Solve Rate: 80%

I wonder what this really is... [enc](Transformation_files/enc) 
''.join([chr((ord(flag[i]) << 8) + ord(flag[i + 1])) for i in range(0, len(flag), 2)])

### Hints
1. You may find some decoders online

### Approach
Open [enc](Transformation_files/enc) using any text editor of your choice (such as Notepad).


### Flag
picoCTF{s4n1ty_v3r1f13d_b5aeb3dd}

---
[Back to home](https://github.com/yanganyi/writeup-picogym)