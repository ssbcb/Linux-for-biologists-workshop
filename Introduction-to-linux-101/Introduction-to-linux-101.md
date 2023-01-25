# Introduction: 
Welcome to Saudi society for Bioinformatics and computational biology (SSBCB)  fisrt workshop. 
Today, we will talk about an introduction to linux for biologist. 

![pic](https://www.genengnews.com/wp-content/uploads/2019/11/Nov1_2019_shutterstock_1084540790_GeneticResearch-e1572877968584.jpg)


## But first, What is the difference between Bioinformatics and computational biology ?? 


### Bioinformatics: 
- Collection and storage of biological informations
- Biological data analysis utilizing computer based tools, softwares ...etc 

### Computational Biology: 
- Development of Algorithms and statistical models to analyze biological data

.



## Bioinformaticians and Bioinformaticist ? 
- Bioinformatician: is a skilled person who only utilize bioinformatics tools and softwares. 

- Bioinformaticist: is a specialist who uses bioinformatics tools and, knows how to write codes and programs. 

------

# Layout: 
workshop series will answer the following questions: 
1.	Introduction to Linux:
    - 	What is Linux and how is it different from other operating systems?
    - Why might a biologist want to use Linux?
    - Overview of the Linux command line interface
2.	Installing and using software:
    - How to find and install software in Linux (MacOS, windows (ubuntu, wsl and VM) 
3.	Basic Linux commands:
    - Navigating the file system
    - Permissions 
    - Creating and managing files and directories 

-----

# 1.	 Introduction to linux:
## a.	What is Linux and how is it different from other operating systems?
Linux is a free and open-source operating system that was developed in the early 1990s. It is based on the Unix operating system and is widely used on servers, desktops, and embedded devices. Unlike proprietary operating systems like Windows and macOS, the source code for Linux is freely available and can be modified and distributed by anyone. makes it a popular choice for developers and technical users who want more control over their computing environment.

For biologists, Linux can be a useful tool for data analysis, simulation, and other tasks that require a high-performance computing environment. It is also often used on remote servers and clusters for running long-term simulations or analyses. 

## b.	Why might a biologist want to use Linux?
There are several reasons why a biologist might want to use Linux:
-	Linux is free and open-source, so there are no licensing fees or restrictions on its use.
-	Linux provides access to a wide range of bioinformatics tools and resources, many of which are available as open-source software
-	It is highly customizable and can be tailored to specific needs or preferences.
-	There are a wide variety of tools and software available for Linux, including many that are specifically designed for scientific research and data analysis.
-	It is stable and reliable, making it a good choice for long-term projects or simulations.
-	Linux has a large and active community of users and developers, so there is a wealth of resources and support available.

## c.	Overview of the Linux command line interface
The command line interface (CLI) is a text-based way of interacting with a computer. In Linux, the CLI is the primary way of issuing commands and interacting with the system. Some basic commands for navigating the file system and manipulating files, directories and running programs. It allows users to enter commands directly into the terminal, rather than using a graphical user interface (GUI) like in Windows or macOS.

----
# 2.	Installing and using software:
## a. Install/acess linux in difeerent os: 
Explain from this: 
https://swcarpentry.github.io/shell-novice/setup.html 

## b.	Acess Linux (MacOS, windows (ubuntu, wsl and virtual machine) 
To access the command line in Linux, you will need to open a terminal window. can usually be done by pressing Ctrl+Alt+T or by searching for "terminal" in the start menu or application launcher.
Once you have a terminal window open, you can enter commands by typing them in and pressing Enter. 

## c. The Shell:

- The shell is a program where users can type commands. With the shell, it’s possible to invoke complicated programs like climate modeling software or simple commands that create an empty directory with only one line of code. The most popular Unix shell is Bash (the Bourne Again SHell — so-called because it’s derived from a shell written by Stephen Bourne). Bash is the default shell on most modern implementations of Unix and in most packages that provide Unix-like tools for Windows. 

When the shell is first opened, you are presented with a prompt, indicating that the shell is waiting for input.
```
$
```
![shell structure](https://storage.googleapis.com/algodailyrandomassets/curriculum/software-engineering/bash-commands/prompt.png) 

- The shell typically uses ``` $ ``` as the prompt, but may use a different symbol. 
- Most importantly: when typing commands, either from this workshop or from other sources, do not type the prompt, only the commands that follow it. Also note that after you type a command, you have to press the Enter key to execute it.
- The prompt is followed by a text cursor, a character that indicates the position where your typing will appear. The cursor is usually a flashing or solid block, but it can also be an underscore or a pipe. You may have seen it in a text editor program.
---

# 3.	Basic Linux commands:
Cheat sheet: A list of basic Linux commands and their usage (e.g. https://www.guru99.com/linux-commands-cheat-sheet.html) 

```
git clone https://github.com/ssbcb/Linux-for-biologists-workshop
```

## a.	Navigating the file system:
![filesystem](https://www.testingdocs.com/wp-content/uploads/Linux-File-System.png)

The file system in Linux is organized into a hierarchy of directories (folders) containing files and other directories, similar to the way folders are organized on a computer. The top-level directory is called the ```"root"``` directory, and is represented by a forward slash (/) on the command line. To change to a different directory, use the ```cd``` command followed by the name of the directory you want to go to. For example, to change to the home directory, you can use the command ``` cd ~ ```
To see the contents of a directory, use the ```ls``` command. You can also use options such ```as -l``` (long format) or ```-a``` (show hidden files) to get more information about the files and directories.

- To go up one level in the directory hierarchy, use the command ```cd ..``

- To go back to the previous directory you were in, use the cd - command.
    - ```cd```   change the current working directory
    - ```pwd```  print the current working directory
    - ```ls ``` list the contents of a directory
    - ```.. ```  move up one directory level
    - ```/  ``` the root directory of the file system

        ![command structure](https://swcarpentry.github.io/shell-novice/fig/shell_command_syntax.svg)


        ![command structure 1](https://static.packt-cdn.com/products/9781800566002/graphics/assets/a1df237d-c2b7-4f48-b917-1dd2bf3d23f8.png)

## b.	Permissions: 
In Linux, the file system is organized in a hierarchical structure, with directories (folders) containing files and other directories. Each file and directory have a set of permissions that control who can access and modify it.
There are three types of permissions in Linux:
- read (r): allows a user to view the contents of a file or directory
- write (w): allows a user to modify the contents of a file or directory
- execute (x): allows a user to execute a file (e.g. a script or program) or traverse a directory (i.e. access its contents)

![permissions](https://www.comentum.com/images/permissions.jpg)

Permissions can be set for three categories of users:
- owner: the user who created the file or directory
- group: a group of users who share access to the file or directory
- other: all other users who do not belong to the owner or group

Permissions can be represented using a combination of letters (r, w, x) or numbers (4, 2, 1). For example, the permission rw-r--r-- can be represented as 644, with the digits representing the permissions for the owner (6), group (4), and other (4).

To view and modify the permissions of a file or directory, you can use the ```chmod``` command. For example, to give the owner read and write permissions, the group read permissions, and other no permissions on a file named myfile, you can use the following command:
```
chmod 640 myfile 
```

You can also use the ``` chown``` command to change the owner of a file or directory, and the ``` chgrp ``` command to change the group ownership.

It's important to carefully manage file permissions in order to maintain the security and integrity of your data. For example, you might want to restrict write permissions to prevent accidental modifications, or limit execute permissions to prevent unauthorized execution of scripts or programs.

https://www.cyberciti.biz/faq/unix-linux-bsd-chmod-numeric-permissions-notation-command/

https://linuxize.com/post/understanding-linux-file-permissions/

## C.	Creating and managing files and directories: 

- Creating and managing files and directories To create and manage files and directories in Linux, you can use the following commands:
    - ```touch``` create a new file
    - ```mkdir``` create a new directory
    - ```cp``` copy a file or directory
    - ```mv``` move or rename a file or directory
    - ```rm``` delete a file or directory
- 	Viewing and editing text files To view and edit text files in Linux, you can use the following commands:
    - ```cat``` display the contents of a text file
    - ```less``` display the contents of a text file one page at a time
    - ```nano``` open a text file in a simple text editor
    - ```vi``` open a text file in a more advanced text editor

-  More explanations and details: 
    - To create a new directory, use the ``` mkdir  ``` command followed by the name of the directory you want to create. For example, ``` mkdir my_dir ``` will create a new directory called "my_dir".
    - To create a new file, use the ```touch``` command followed by the name of the file you want to create. For example, ```touch my_file.txt``` will create a new text file called "my_file.txt".
    - To copy a file, use the ```cp``` command followed by the source file and the destination. For example, ```cp my_file.txt ```, my_file_copy.txt will create a copy of "my_file.txt" called "my_file_copy.txt".
        - here talk about the -rf commands in general 
    - To move or rename a file, use the``` mv``` command followed by the source file and the destination. For example, ```mv my_file.txt my_dir/my_file.txt ``` will move "my_file.txt" to the "my_dir" directory, and ```mv my_file.txt my_file_newname.txt ``` will rename "my_file.txt" to "my_file_newname.txt".


----
# Extra resorces: 
- https://swcarpentry.github.io/shell-novice/ 
- https://explainshell.com/explain?cmd=ls+-l 

