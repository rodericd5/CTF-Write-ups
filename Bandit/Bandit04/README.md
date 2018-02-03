**Task:** The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

**Clue:** The only file that has all human readable characters provides the password

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

**Solution:** `for file in ~/inhere/*; do cat $file; printf "\n"; done` this is a simple script that iterates through all of the files in the directory and reads them, separating them by newlines each time. It prints a newline each time so you can easily discern the results. The alternative would be to cat each file individually by hand
