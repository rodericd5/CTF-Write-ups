**Task:** The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

**Clue:** Look at the ssh man pages and figure out how to pass a private key as an argument

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

**Solution:** 
`ssh -i sshkey.private bandit14@localhost` this logs you in to bandit14 using the localhost

`cd /etc/bandit_pass/bandit14; cat bandit14` This reads the file and outputs the password to the console!
