# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](https://web.archive.org/web/20160708171659/http://cli.learncodethehardway.org/book/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. Each "chapter" focuses on a command. Type the commands you see in the _Do This_ section, and read the _You Learned This_ section. Move on to the next chapter. You should be able to go through these in a couple of hours.

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

> > * pwd: prints the current directory
	* mkdir: creates a directory
	* rmdir: removes a directory 
	* touch: creates a file
	* rm: deletes a file
	* mv file1.txt file2.txt: renames file1 to file2
	* ls -a: list all files including hidden files
	* cp dir/file.txt dir2/file.txt: copies file to new directory
	* grep: allows you to search files that contain a pattern
	* cat: prints file contents to standard output

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

> > `ls`: lists all files and directories within the working directory.
`ls -a`: displays all files including hidden files
`ls -l`: displays files in long format table
`ls -lh`: displays long format with human friendly units for file size
`ls -lah`: displays long format with hidden files and friendly units for file size 
`ls -t`: sort files by time
`ls -Glp`: displays long format listing excluding owner name with trailing `/`

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > Favorites:
	* -a
	* -d
	* -u
	* -l
	* -1

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > `xargs` is a command that is typically used where the output of one command is passed as arguments to another command. An example would be creating files from a list present in a text file. Assuming you have a file called `test.txt` and it contains two lines. Those lines are:
`file1.txt`
`file2.txt`
Writing the following in the command like would create two files named `file1.txt` and `file2.txt`.
`cat test.txt | xargs touch`

 

