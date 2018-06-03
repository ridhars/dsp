# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

```
pwd : print working directory
mkdir : create directory
rmdir : delete empty directory
touch : create a file
rm    : delete a file
mv    : rename or move a file
ls -a : list all including hidden files
cp    : copy a file
cd    : change directory
chmod : change permission
```

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

```
ls    : list files
ls -a : list all files
ls -l : list files with long detail
ls -lh: list files with 'human readable' detail
ls -lah : list all files with 'human readable' detail
ls -t    : list files ordered on creation time
```
---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

```
ls -a : all files
ls -t : ordered by creation time
ls -p : directories with /
ls -R : show subdirectories
ls -l : long format
```

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

>>>
xargs are usually used to pass **a multiple or long list** into another command

e.g. (as taken from Wikipedia): chaining xargs with rm to **remove list of files**

find . | xargs rm

 

