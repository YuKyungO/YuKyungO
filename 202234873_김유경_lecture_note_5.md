# Shell Command
### I/o Redirection : Standard Output
- \>   
    To create and save the output in a file.       
    Ex) $ ls -lh **\>** file_list.txt
- cat  
    Displays the content of a text file.       
    Ex) $ **cat** file_list.txt
- \>\>   
    If it already exitsts appends output to an extising file, or create and write to a new file is it doesn't exist.       
    Ex) $ ls -lh **\>\>** file_list.txt   

### I/o Redirection : Standard Input
< : Redirecct input    

### Pipelines
- **|** : Feeds output of previous command to input of next command. Press 'q' key to exit the screen.   
    Ex) command1 | command2 | command3 | ...

- **| wc -l** : Number of files in the current directory   
    Ex) $ ls | wc -l   
    7

### Expansion   
▷    Special characters expand its meaning when given to shell commands.    
Ex) $ **echo** print out the text     
print out the text    

Ex) $ **echo \***     
(Output files in the current directory)

Ex) $ **echo ~**    
(Output the current user's home directory)

### Permissions
*-rwxrwxrwx*    
- \- : indicates regular file    
- d : indicates directory        

    'rwx' means 'Read, write, and execute' in order.     
    Files and directories have a permission assigned differently to owner / group / others.      

*chmod* : Changes permissions.     
Ex) $ **chmod** 600 some_file      
rwx rwx rwx = 111 111 111      
rw- rw- rw- = 110 110 110      
rwx --- --- = 111 000 000        

### Superuser    
A superuser has all system administation authority.      
Put 'sudo' before the command if you are a superuser.       
Ex) $ **sudo** some_command        

### Text Editors   
In Linux, you can choose CLI-based or GUI-based text editors.    
*[Name] : [Interface]*        
- vi, vim : command line     
- Emacs : command line    
- nano : command line    
- gedit : graphical    
- kwrite : graphical      

### Shell Script    
Write and run a shell script.     
Ex) $ nano myscript . sh     

---

##### **Tip**    
- **Backslash** : Can be used to ignore line change in command ('enter'), to enter a long command in multiple lines.       
    Ex) $ ls -l \\      
    \> --reverse \\      
    \> --human-readable      

- **History** : To see previous command history or save it to a text file.      
    Ex) $ history \> history_command.txt     
    $ cat history_command.txt     