**Task:** The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

**Clue:** First worry about reversing the hexdump, then try to find out how the file it produces was zipped and go one step at a time.

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
`mkdir /tmp/folderHolder; scp data.txt /tmp/folderHolder; cd /tmp/folderHolder` these are three separate commands for first making the directory, then copying the data.txt file to it, and finally changing to the directory.

`xxd -r data.txt > tempFile; file tempFile` This reverses the hexdump and then puts it into a new file called tempFile. The second command checks what file type tempFile is.
 
 The file command told me that it was a gzip and so we should add the appropriate extension and then unzip it.
 
`mv tempFile tempFile.gz; gunzip tempFile.gz`

This process continues for several more unzips of different filetypes such as bzip, gzip, and tar files. Each one has its own method of being unzipped, but syntax aside the method for solving this problem is outlined above: rename the file with appropriate extension and perform the appropriate method of unzipping.

