## Level Goal

The password for the next level is stored in a file called spaces in this filename located in the home directory.

## Commands you may need

* `ls`: List directory contents
* `cd`: Change directory
* `cat`: Concatenate and print files
* `file`: Determine file type
* `du`: Display disk usage
* `find`: Search for files

## Results

```
bandit1@bandit:~$ ls -lhart
total 24K
-rw-r--r--  1 root    root     807 Mar 31 08:41 .profile
-rw-r--r--  1 root    root    3.7K Mar 31 08:41 .bashrc
-rw-r--r--  1 root    root     220 Mar 31 08:41 .bash_logout
drwxr-xr-x  2 root    root    4.0K Jul 17 15:57 .
-rw-r-----  1 bandit2 bandit1   33 Jul 17 15:57 -
drwxr-xr-x 70 root    root    4.0K Jul 17 15:58 ..
bandit1@bandit:~$ cat "-"
^C
bandit1@bandit:~$ cat ./-
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
bandit1@bandit:~$

``` 

## Explicacao 

Utilizeo o `./` para determinar o local do qual estava realmente executando o cat, quando estamos trabalhando com esses nomes nao absolutos
O O.S tem problemas para interpretar caminho.
