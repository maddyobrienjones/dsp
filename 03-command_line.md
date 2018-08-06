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

> > `pwd`: show current working directory path
> > `mkdir [directory]`: creating a directory
> > `rm [directory]`: deleting a directory
> > `touch [file]`: creating a file
> > `rm [file]`: deleting a file
> > `mv [file] [newname]`: renaming a file
> > `ls -a`: listing hidden files
> > `cp [directory1]/[file] [directory2]/`: copying a file from one directory to another
> > `mv [file] [directory]/`: moving a file from working directory to another
> > `cp a*.txt [directory]/`: copies all .txt files starting with a in working directory to `[directory]`

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

> > `ls`: lists files in working directory
> > `ls -a`: displays all files, including hidden files
> > `ls -l`: lists contents in long format
> > `ls -lh`: prints files in long format with sizes in human-readable format
> > `ls -lah`: prints all files in long format with sizes in human-readable format
> > `ls -t`: lists files sorted by timestamp
> > `ls -Glp`: lists contents in long format, displays directories with / in front, doesn't print group names

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > `ls -1`: displays each entry on a line
> > `ls -c`: displays file by file timestamp
> > `ls -u`: displays file by file access time
> > `ls -m`: displays names as comma-separated list
> > `ls -R`: displays subdirectories as well

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > `xargs` takes in a command, and then takes in an argument from standard input to run the command. An example would be `xargs find -name`. This opens up standard input, where you could put in a*.txt. This would search the working directory for all txt files starting with 'a'.
