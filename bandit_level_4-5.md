## Level Goal

The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

## Commands you may need

* `ls`: List directory contents
* `cd`: Change directory
* `cat`: Concatenate and print files
* `file`: Determine file type
* `du`: Display disk usage
* `find`: Search for files

## Results

```
bandit3@bandit:~$ ls -lhart
total 24K
-rw-r--r--  1 root root  807 Mar 31 08:41 .profile
-rw-r--r--  1 root root 3.7K Mar 31 08:41 .bashrc
-rw-r--r--  1 root root  220 Mar 31 08:41 .bash_logout
drwxr-xr-x  3 root root 4.0K Jul 17 15:57 .
drwxr-xr-x  2 root root 4.0K Jul 17 15:57 inhere
drwxr-xr-x 70 root root 4.0K Jul 17 15:58 ..
bandit3@bandit:~$ cd inhere/
bandit3@bandit:~/inhere$ ls -lhart
total 12K
drwxr-xr-x 3 root    root    4.0K Jul 17 15:57 ..
-rw-r----- 1 bandit4 bandit3   33 Jul 17 15:57 ...Hiding-From-You
drwxr-xr-x 2 root    root    4.0K Jul 17 15:57 .
bandit3@bandit:~/inhere$ cat ./.
./                  ../                 ...Hiding-From-You  
bandit3@bandit:~/inhere$ cat ./.
./                  ../                 ...Hiding-From-You  
bandit3@bandit:~/inhere$ cat ./.
./                  ../                 ...Hiding-From-You  
bandit3@bandit:~/inhere$ cat ./...Hiding-From-You
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
 
```

Explicacao

Ao utilizar o `ls -lhart` o paramentro `-a` e responsavel por mostrar todos os arquivos ocultos.
