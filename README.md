# Small cryptography program

This program is designed to either encode or decode messages using either a Caesar cipher or a Vigenere cipher. The program is written in Python, but must be run via JupyterLab as it is housed in a Jupyter notebook file. Written for Lab 6 exercise of UPitt's CMPINF0010 course.

# Getting started

Instructions on how to install and use JupyterLab can be found [here](https://docs.google.com/document/d/1zYiZpnU86_bE2qfRYLke1lAxukKCpO6idhv-hUQafpU/edit). 
After installing JupyterLab:

1. Start the terminal in JupyterLab
2. Find the folder you would like to download the program to
3. Enter in the command git clone https://github.com/zogerreng/Small-cryptography-program
4. Find the folder named "small-cryptography-program" and launch the ipynb file inside

# How to actually use the program

When you run the ipynb file, you will:

1. Choose between a Caesar or Vigenere cipher, by either entering in the number "1" or "2" (respectively)
2. Choose between encoding or decoding, by either entering in the number "1" or "2" (respectively)
3. Enter a string to either decode or encode.
4. Depending on whether you chose a Caesar or Vigenere cipher:
  - You will enter the Caesar shift, which can be any integer
  - You will enter a Vigenere key, which is any string with only alphabetical characters in it.

If any of your inputs do not match for each step, the program will not function and you will have to restart it.

# Caesar and Vigenere ciphers explained

## Caesar explained

Each letter of the alphabet can be mapped to a number: "a" with 0, "b" with 1, all the way to "z" with 25 (zero-indexed). Because we can assign a number to every alphabetical letter, a Caesar cipher can shift each letter in a given plaintext by a specific integer amount. This is done by adding the shift to the number corresponding with each letter in the string. For example, take the plaintext "abc". Represented as 012 with a given Caesar shift of 3, 012 becomes 345 becomes "def". In the case that the number added with the shift is greater than 25 (goes past the end of the alphabet), the shift will loop back around from the beginning of the alphabet. For example, the letter "z" shifted 2 becomes "b". 

Video explanation [here.](https://www.youtube.com/watch?v=sMOZf4GN3oc)

## Vigenere explained

Again, each letter of the alphabet can be mapped to a number: "a" with 0, "b" with 1, all the way to "z" with 25 (zero-indexed). In the case of a Vigenere cipher, a specific string key is used to encode the plaintext. This key is used to determine the shift for each letter. Take plaintext "abcdefg" with key "test" for example. The key is written so that each letter of the key lines up with its corresponding letter in the plaintext. If the plaintext is larger than the key, the key is repeated multiple times. With our plaintext "abcdefg" and key "test", the key written out with the plaintext would look like "testtes".

![whyamistillworking](https://user-images.githubusercontent.com/22896094/110892833-c8db1780-82c2-11eb-8e47-35f850f44c0e.PNG)

Notice how each letter lines up with a letter of the plaintext. Each letter in the plaintext is shifted by the amount in the key. Starting at the first letter, "a": "a" would be shifted over 19 spots because "t" corresponds with the number 19. The next letter, "b" would be shifted over 5 spots because "e" corresponds with the number 5. This continues with each letter of the plaintext.

In case the explanation didn't make sense (it probably didn't) and you actually want to understand it, a video explanation can be seen [here.](https://www.youtube.com/watch?v=zNO4PTlg62k)

# Wonderful contributors + how to contact us

If you have any questions about the program and how it works, or if you'd like to report a bug, please feel free to contact any of us. 

1. Roger Zeng (roz30@pitt.edu)
2. Julia Livingston (jul126@pitt.edu)
3. Brady Snyder (bcs66@pitt.edu)



