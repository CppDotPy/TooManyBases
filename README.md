# TooManyBases

This project has 3 functions.

|exponent|
This function takes 2 input; base and exponent.
The function raises the base to the power of the exponent.
note: it only works on positive intagers and 0.

|standardise|
This function takes 2 inputs and an arbitrary key word argument; base, num and **map.
Then function uses the formula Σb^{n}x=d to convert a given number num of base base,
to base 10. For bases higher than 10 you can use **map to asign characters to numbers
above 9.

e.g.
To convert from hexadecimal (base 16) to base 10, the standard is to use a - f to
reprisent numbers 10 - 15. To achive this result you would use:
standardise(16, "{num}", a=10, b=11, c=12, d=13, e=14, f=15)

The **map kwarg can also be used to reprisent numbers of higher bases in base 10.
Where the size determins what the program conciders one number.

e.g.
standardise(16, "2f", a=10, b=11, c=12, d=13, e=14, f=15)
Could also be written as:
standardise(16, "0215", size=2)

In the example above the program treats every pair of two digits as one digit,
therefore eliminating the need to assign characters to numbers

|conversion|
This function takes 3 variables and a kwarg, fbase, tbase, num and **map.
fbase Reprisents the base of the number you want to convert, tbase reprisents
the base you want to convert the number to, and num is the number you want to
convert. **map Is used the dame as in |standardise|.


This program was origianally written to work with time, as time works with
base 60 reprisented in base 10.

I hope that the README file made sense and I hope you enjor my first ever github project!!!
