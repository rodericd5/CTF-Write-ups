**Task:** The password for the next level is stored in the file data.txt, which contains base64 encoded data.


**Clue:** read up on base64 and then check the manual pages

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

**Solution:** `cat data.txt | base64 --decode` cat the data file and pipe the output to base64 and decode it

