---
title: Frequent Used Commends
date: 2020-12-04
categories: [Coding, General]
tags: [ENG]     # TAG names should always be lowercase
---

*Cheat Sheet for frequent used commends*

## Unix

### tar
-c create \\
-x extract \\
-t, –list – list the contents of an archive

-v verbose \\
-f filename \\
-z gzip \\
-j bzip2

```bash
tar -cvf songs.tar Ukulele/
tar -cvzf songs.tar.gz Ukulele/
tar -cvjf songs.tar.bz2 Ukulele/

tar -xvf songs.tar
tar -xvzf songs.tar.gz
tar -xvjf songs.tar.bz2
```

### uname

see system information

-a all \\
-s kernel name \\
-r relsase \\
-v kernel version

### mkdir

-p no error if existing, make parent directories as needed

### sftp

like ssh \\
lls local ls \\
put upload \\
-r recursive \\

```bash
sftp username@discovery.usc.edu
Connected to discovery.usc.edu.
sftp> lls 
md.c md.h md.in
sftp> cd cs596
sftp> put md.*
sftp> put -r ~/user/folder
sftp> ls
md.c md.h md.in
sftp> exit
```

### rm

-f force\\
-r recursive\\
-v verbose

### split

-l linenumber\\
-b bytes

```bash
split -b 40k myfile segment
cat segment* > myfile
```

### head
-n number of lines
