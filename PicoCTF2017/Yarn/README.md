# Task:
I was told to use the linux strings command on yarn, but it doesn't work. Can you help? I lost the flag in the binary somewhere, and would like it back

### Hints (Given):
What does the strings command use to determine if something is a string?
Is there an option to change the length of what strings considers as valid?

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

After downloading the Yarn binary, I attempt to use strings on it and see that it does not in fact work. I decided to cat yarn and see if it would provide me with anything. It's a total mess and not all of it is even printable to the console, so following with their hint I decide to try a modified strings command

`strings - -n 8 yarn` This makes string search for everything, and since the hint asks about length I decided to change the initial size requirement to 8 bytes instead of 4. 

This turns out a lot of readable stuff, but nothing particularly useful, so I decide to go the other way with it.

`strings - -n 2 yarn`AHA! Somewhere in the middle of the output we can clearly see the flag! 
