**Task:** The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions


**Clue:** look into the tr command and how it can be used to "shift" characters

S

P

O

I

L

E

R

A

L

E

R

T

!

**Solution:** `cat data.txt | tr ['A-Z'] ['N-ZA-M'] | tr ['a-z'] ['n-za-m']` cat the data file and pipe the output to tr shifts for upper and lowercase letters. 
Note how A's map to N's (13 letters away) and this process continues until you map an M to a Z at which point the characters start mapping to A through M. 
This logic holds for both upper and lowercase letters.

