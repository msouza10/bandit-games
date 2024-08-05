## Level Goal

The password for the next level is stored in a file called **readme** located in the home directory.

## Commands you may need

* `ls`: List directory contents
* `cd`: Change directory
* `cat`: Concatenate and print files
* `file`: Determine file type
* `du`: Display disk usage
* `find`: Search for files

## Results

```
bandit0@bandit:~$ pwd
/home/bandit0
bandit0@bandit:~$ ls -lhart
total 24K
-rw-r--r--  1 root  root  807 Mar 31 08:41 .profile
-rw-r--r--  1 root  root  3.7K Mar 31 08:41 .bashrc
-rw-r--r--  1 root  root  220 Mar 31 08:41 .bash_logout
-rw-r-----  1 bandit1 bandit0 437 Jul 17 15:57 readme
drwxr-xr-x  2 root  root  4.0K Jul 17 15:57 .
drwxr-xr-x 70 root  root  4.0K Jul 17 15:58 ..
bandit0@bandit:~$ cat readme
Congratulations on your first steps into the bandit game!!
Please make sure you have read the rules at https://overthewire.org/rules/
If you are following a course, workshop, walthrough or other educational activity,
please inform the instructor about the rules as well and encourage them to
contribute to the OverTheWire community so we can keep these games free!

The password you are looking for is: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

bandit0@bandit:~$ 
``` 
