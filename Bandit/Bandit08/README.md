**Task:** The password for the next level is stored in the file data.txt and is the only line of text that occurs only once


**Clue:** uniq will be useful for determining repeats, but the data needs to be sorted first

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

**Solution:** `sort -n data.txt | uniq -u` perform a numerical sort on the data and pipe the output to uniq -u which will print only text that occurs once.

