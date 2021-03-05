# CMPINF-0010_Lab5Exercise
program with do_something

This program takes in a string input and an integer input. Using do_something, it converts the string to lowercase, then shifts each letter in the given string over by the integer input (it performs a Caesar shift). For example: given a string input 'abc' and an integer input of 3, the output string would be 'def'. Because each letter in the alphabet corresponds to a number (a = 0, b = 1, etc.) we can shift each letter over by a certain amount. 

To do this, each letter is converted to its respective ASCII code. Next, 97 is subtracted from each code because we want each letter to be between 0-25, and lowercase 'a' corresponds with 97 in the ASCII table. The new code gets the shift added to it, then is modded by 25. Finally, 97 is added back to the code and the code is converted back to a letter. 

After do_something is executed, the results are printed.

# Group members:

1. Roger Zeng
2. Julia Livingston
