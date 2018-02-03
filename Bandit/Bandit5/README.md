**Task:** The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable

1033 bytes in size

not executable

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

**Solution:** `find . -size 1033c ! -executable -exec cat {} +` It is worth noting that this solution does not take into account the fact that the file should be human-readable, but that is a somewhat ambiguous property and we would have to make assumptions in order to search for a particular filetype. There is only one 1033 byte non executable in the inhere directory so this solution works.
