# Linux
Open-source Unix-like operating systems and kernels.   
Runs on CLI (Command Line Interface), but many distributions support GUIs as well.

#### Kernel and Shell
Kernel : Core of OS that controls and communicates with hardware resource.   
Shell : Interface that allows users to communicate with kernel. Users runs applications and give commands through shell.

# Shell command
1. pwd : shows the current path in a hierarchical directory   
2. cd : change directory
3. ls : list files and directories    

---
####  cd and ls    
*arguments*
    
```sh
    /   root
    .   current directory
    ..  upper-level directory
    ~   home of current user
    /[directory name] : absolute path
    ./[directory name] : relative path
    ../[directory name] : relative path
```

*options*
    
 ```sh
     -l : show detailed information (long format)
     -lh : same as -l, but size in units
```

---

*ls*
```sh
    $ ls : list the files in the working directory
    $ ls /bin : list the files in the /bin directory (or any other directory we care to specify)
    $ ls -l : list the files in the working directory in long format
    $ ls -l /etc /bin : list the files in the /bin directory and the /etc directory in long format
    $ ls -la .. : list all files (even ones with names beginning with a period character, which are normally hidden) in the parent of the working directory in long
```
---
4. cp : copy files and directories
```sh
$ cp file1 file2 : copies the contents of file1 into file2. If file2 does not exist, it is created; otherwise, file2 is silently overwritten with the contents of file1.
$ cp -i file1 file2 : like above however, since the "-i" (interactive) option is specified, if file2 exists, the user is prompted before it is overwritten with the contents of file1.
$ cp file1 dir1 : copy the contents of file1 (into a file named file1) inside of directory dir1.
$ cp -R dir1 dir2 : copy the contents of the directory dir1. If directory dir2 does not exist, it is created. Otherwise, it creates a directory named dir1 within directory dir2.
```
5. mv : move files and directories or rename them
```sh
$ mv file1 file2 : If file2 does not exist, then file1 is renamed file2. If file2 exists, itscontents are silently replaced with the contents of file1.
$ mv -i file1 file2 : like above however, since the "-i" (interactive) option is specified, if file2 exists, the user is prompted before it is overwritten with the contents of file1. 
$ mv file1 file2 dir1 : the files file1 and file2 are moved to directory dir1. If dir1 does not exist, mv will exit with an error.
$ mv dir1 dir2 : If dir2 does not exist, then dir1 is renamed dir2. If dir2 exists, the directory dir1 is moved within directory dir2.
```
6. rm : delete files and directories permantely and irreversevely
```sh
$ rm file1 file2 : delete file1 and file2
$ rm -i file1 file2 : like above however, since the "-i" (interactive) option is specified, the user is prompted before each file is deleted.
$ rm -r dir1 dir2 : directories dir1 and dir2 are deleted along with all of their contents.
```
7. mkdir : make a new directory
8. help : provides information on built-in commands
9. man : manual output for commands

#### Wildcards
```sh
    $ * : All filenames
    $ g* : All filenames that begin with the character "g"  
    $ b*.txt : All filenames that begin with the character "b" and end with the characters ".txt"
    $ Data??? : Any filename that begins with the characters "Data" followed by exactly 3 more characteres
```