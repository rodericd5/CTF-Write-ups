**Task:** The password for the next level is stored in the file data.txt in one of the few human-readable strings, beginning with several ‘=’ characters.


**Clue:** strings can read binary files and what the task means by human-readable is really that it's a string

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

**Solution:** `strings data.txt | grep "======"` use strings to read human-readable info and pipe the result to grep looking for a few "="

