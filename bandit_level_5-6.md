## Level Goal

The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable
1033 bytes in size
not executable

## Commands you may need

* `ls`: List directory contents
* `cd`: Change directory
* `cat`: Concatenate and print files
* `file`: Determine file type
* `du`: Display disk usage
* `find`: Search for files

## Results

```
bandit4@bandit:~$ ls -lhart
total 24K
-rw-r--r--  1 root root  807 Mar 31 08:41 .profile
-rw-r--r--  1 root root 3.7K Mar 31 08:41 .bashrc
-rw-r--r--  1 root root  220 Mar 31 08:41 .bash_logout
drwxr-xr-x  3 root root 4.0K Jul 17 15:57 .
drwxr-xr-x  2 root root 4.0K Jul 17 15:57 inhere
drwxr-xr-x 70 root root 4.0K Jul 17 15:58 ..
bandit4@bandit:~$ cd inhere/
bandit4@bandit:~/inhere$ ls -la
total 48
drwxr-xr-x 2 root    root    4096 Jul 17 15:57 .
drwxr-xr-x 3 root    root    4096 Jul 17 15:57 ..
-rw-r----- 1 bandit5 bandit4   33 Jul 17 15:57 -file00
-rw-r----- 1 bandit5 bandit4   33 Jul 17 15:57 -file01
-rw-r----- 1 bandit5 bandit4   33 Jul 17 15:57 -file02
-rw-r----- 1 bandit5 bandit4   33 Jul 17 15:57 -file03
-rw-r----- 1 bandit5 bandit4   33 Jul 17 15:57 -file04
-rw-r----- 1 bandit5 bandit4   33 Jul 17 15:57 -file05
-rw-r----- 1 bandit5 bandit4   33 Jul 17 15:57 -file06
-rw-r----- 1 bandit5 bandit4   33 Jul 17 15:57 -file07
-rw-r----- 1 bandit5 bandit4   33 Jul 17 15:57 -file08
-rw-r----- 1 bandit5 bandit4   33 Jul 17 15:57 -file09
bandit4@bandit:~/inhere$ file ./*
./-file00: data
./-file01: data
./-file02: data
./-file03: data
./-file04: data
./-file05: data
./-file06: data
./-file07: ASCII text
./-file08: data
./-file09: data
bandit4@bandit:~/inhere$ cat ./-file0
cat: ./-file0: No such file or directory
bandit4@bandit:~/inhere$ cat ./-file07
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
bandit4@bandit:~/inhere$ 
```

## Notes

O comando `file` determina os tipos de arquivo, como uma das dicas foi que o arquivo era `human-readable`, ficou obvio que o output seria ASCII
