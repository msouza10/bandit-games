## Level Goal

The password for the next level is stored in a hidden file in the inhere directory.

## Commands you may need

* `ls`: List directory contents
* `cd`: Change directory
* `cat`: Concatenate and print files
* `file`: Determine file type
* `du`: Display disk usage
* `find`: Search for files

## Results

```
bandit2@bandit:~$ ls -lhart
total 24K
-rw-r--r--  1 root    root     807 Mar 31 08:41 .profile
-rw-r--r--  1 root    root    3.7K Mar 31 08:41 .bashrc
-rw-r--r--  1 root    root     220 Mar 31 08:41 .bash_logout
-rw-r-----  1 bandit3 bandit2   33 Jul 17 15:57 spaces in this filename
drwxr-xr-x  2 root    root    4.0K Jul 17 15:57 .
drwxr-xr-x 70 root    root    4.0K Jul 17 15:58 ..
bandit2@bandit:~$ cat "spaces in this filename" 
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

```

## Notes

Utilizando o comando `cat "spaces in this filename"` estou protejendo nome para o shell conseguir interpretar o nome do arquivo de forma correta.

outra abordagem que tambem seria possivel, seria utilizadar o cat anterior `cat ./` e o nome do arquivo.

