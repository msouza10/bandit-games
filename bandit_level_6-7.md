## Level Goal

The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size

## Commands you may need

* `ls`: List directory contents
* `cd`: Change directory
* `cat`: Concatenate and print files
* `file`: Determine file type
* `du`: Display disk usage
* `find`: Search for files
* `grep`: Print lines that match patterns

## Results

```
bandit5@bandit:~$ cd inhere/
bandit5@bandit:~/inhere$ ls -la * |grep "1033"
-rw-r-----  1 root bandit5 1033 Jul 17 15:57 .file2
bandit5@bandit:~/inhere$ find ./* -size 1033
bandit5@bandit:~/inhere$ find ./ -size 1033
bandit5@bandit:~/inhere$ find ./ -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$ find ./ -size 1033c | cat
./maybehere07/.file2
bandit5@bandit:~/inhere$ cat ./maybehere07/.
./      ../     .file1  .file2  .file3  
bandit5@bandit:~/inhere$ cat ./maybehere07/.
./      ../     .file1  .file2  .file3  
bandit5@bandit:~/inhere$ cat ./maybehere07/.file
.file1  .file2  .file3  
bandit5@bandit:~/inhere$ cat ./maybehere07/.file02
cat: ./maybehere07/.file02: No such file or directory
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2 
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
bandit5@bandit:~/inhere$ ^C
```

## Notes

Realizei a filtragem do arquivos utilizando como base o size do arquivo no comando find e o parametro `-size`.
