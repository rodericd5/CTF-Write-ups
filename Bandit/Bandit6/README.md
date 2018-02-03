**Task:** The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7

owned by group bandit6

33 bytes in size

**Clue:** checkout the manual for find to see all of the ways you can modify a search

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

**Solution:** `find / -group bandit6 -user bandit7 -size 33c -exec cat {} +` This task was similar to the previous one. It attempts to cat every file matching this description (many of which we do not have permission to cat). The last one ends up being the answer

