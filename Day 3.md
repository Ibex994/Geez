# 1)Information gathering
- Tools for information gathering,in system,network, host
    * dmitry
    * ike-scan
    * legion
    * maltego(most used)
    * netdiscover
    * nmap(most used)
    * pof
    * recon-ng(most used)
    * spiderfoot

# 2) Vulnerability Analysis
- Tools for Finding Vulnerabilities
    * legion
    * lynis
    * nikto(most used)
    * nmap (most used)
    * unix-prives

# 3) Web Application Analysis
- Tools for Finding Vulnerabilities and exploits on websites.
    * wpscan
    * burpsuite
    * commix
    * sqlmap(most used)
    * ZAP
    * httrack

# 4) Database Assessment
- Tools for Finding Vulnerabilities and exploits on Databases.
    * jsql-injector
    * mdb-sql
    * oscanner
    * sqldict
    * sqlmap
    * sqlninja
    * sqlsus
# 5) Password Attacks
- Tools for exploiting Passwords for login,websites,application,windows.
    * cewl
    * jhon
    * rainbowcrack
    * ncrack
    * medusa
    * ophcrack
    * wordlist

# 6) Wireless Attacks
- Tools for exploiting Wireless Systems like wifi, bluetooth..
    * aircrack ng
    * chirp
    * cowpatty
    * fern wifi cra...
    * kismet
    * mdk3
    * mfoc
    * mfterm
    * pixiewps
    *  reaver
    * wifite

# 7) Reverse Engineering
- Tools for exploiting Softwares, Mobile Applications and any binary files
    * apktool 
    * bytecode-vi
    * clang
    * clang++
    * dex2jar
    * edb-debug
    * ghidra
    * Jadx-gui
    * javasnoop
    * NASM shell
    * ollydbg
    * radare2

# 8) Eploitation Tools
- Tools for exploiting Softwares, Mobile ,Computers ,websites and any things.
    * armitage
    * beef xss frs
    * searchsploit
    * sqlmap
    * termineter

# 9) Sniffing and Spoofing
- Tools to sniff network traffic or perform IP spoofing attacks.
- Tools for listening or hijacking networks.
    * driftnet
    * hamster
    * mitmproxy
    * respponder

# 10) POST Exploitation
- Tools that aid in maintaining access to a compromised system after an attack has been executed.
    * backdoor-f
    * exe2hex
    * nishang
    * powersploit
    * weevely

# 11) Forensic
- Tools used to analyze digital evidence from computers, mobile devices, servers, etc.
    * autopsy
    * binwalk
    * galleta
    * bul_extrac
    * foremost
    * hashdeep

# 12) Reporting tools
- Tools used to generate reports on vulnerabilities found during penetration testing.
    * maltego
    * pipal
    * recordmyd
    * cutycapt

# 13) Social Engineering tools
- Tools Used for Social Engineering attacks.
    * maltego
    * msf payloa
    * backdoor-f...

# 14) System Services
- Tools related to managing Windows services (services.msc).
    * beef stop
    * beef start
    * dradis start
    * dradis stop

# 15) Usually used applications
- Applications commonly used by security professionals and researchers.

# Workspace manager
- Used to Classify our works on different windows

# LINUX COMMANDS
- Linux Systems uses shell. The shell help us to Communicate with the kernel and helps to execute codes.
**Shell also called “Terminal”**

(rexder@HunterMachine)-[~]
$
- The terminal have 5 parts.
     * Username = rexder
     * Hostname = HunterMachine
     * Current Directory = PATH
     * Priviledge = $-(user) , #-(root)
     * Command place = _
     * Home directory is ~
     * Local directory with .
     * All directory `*`

**Directory = folder**

- On linux there are over 100 commands. But we will see the main and the useful only.
- Also those commands have their own options and arguments.

# What is command?
- A command in Unix or Linux systems is a program that performs a specific task, such as displaying file.
- Small programs that do one task well.

# ls / List Directory
- SYNOPSIS
       `ls [OPTION]... [FILE]...`
## DESCRIPTION
       - List  information  about  the FILEs (the current directory by default).

`ls -l`
`ls -a`
`ls filename`
`ls -R   => recursive`
- You can combine them, ls -Rla
**Linux hidden files start with dot.**

# cd / Change Directory
- SYNOPSIS
     `cd [directory]`
## DESCRIPTION
- It is used to change current working directory. 
- If no argument is supplied, it defaults to home directory.
        `cd/ =>root`
        `cd =>home`
        `cd .. => 1x Back`
        `cd ../.. => 2x Back`
        `cd foldername` 
- If folder name have space you have to add the name inside “ folder name “
	**cd “folder name”**

# pwd / Print Working Directory
- SYNOPSIS
       `pwd [-options]`
## DESCRIPTION
- It prints the path of the working directory, starting from the root.

# echo
- The echo utility writes any specified operands to standard output.
- SYNOPSIS
       `echo [option] [string]`
## DESCRIPTION
- echo command in linux is used to display line of text/string that are passed as an argument . This is a built in command that is mostly used in shell scripts and batch files to output status text to the screen or a file. 
- You can write texts into files.
`echo text > file.txt`
- You can add texts(append)
`echo text >> file.txt`

# cat/head/tail/less
- They are used to read and print the contents of a file.
- SYNOPSIS
`cat [file]`
- Display or concatenate FILEs; also display FILEs whose names match PATTERN. With more than one FILE, precede each with a header showing the file name. When reading, equivalent to ‘-’, but not when writing.
## DESCRIPTION
- Used to show the content of a file.

# cat
- Display contents of file(s).
- SYNOPSIS
`cat filename`
- It displays the content of the file on the console.

# nano
- A small and free text editor.
- SYNOPSIS
`nano filename`
- Opens a new file or edits an existing one using the Nano Editor.

# man
- Display system manual pages.
- SYNOPSIS
`man command_name`
- Displays the manual page entry for COMMAND_NAME.
- The manual page entries are organized by section number, which is followed by a single letter code indicating

# Touch
- SYNOPSIS
`touch filename[s]`
## DESCRIPTION
- This command is used to create a new empty file named as 'filename' in the present working directory if it does not exist already. Otherwise, it updates the timestamp of the existing file.
- This command is used to create a new empty file named as 'filename' in the present working
- Creates any kind of Files with the name you gave it. With empty inside.

# Mkdir / make directory
- SYNOPSIS
`mkdir directoryname`
- Create a new directory called "directoryname" in the current location.
## DESCRIPTION
- Creates Folder with the name u gave it.
- DON’T forget to add the “ “ when you are using folders with space between them.

# clear
- SYNOPSIS
`clear`
- Clears the terminal screen.

# rm / remove
- SYNOPSIS
`rm filename`
- Remove (delete) the file named ‘filename'.
- `rm -r`   => recursive(4 folders)
- `rm -i`    => for prompt(ask)
- `rm -f`    => force delete
- You can use them in combination too like,`rm -rf ‘filename’`

# Cp| mv  / copy,move
- cp : Copy files and directories.
- SYNTAX:
`cp [oldFILEplace] [newfilePlace]`
`Mv  [oldFILEplace] [newfilePlace]`
## DESCRIPTION
- Copy/move  files & folders.

# grep - global search for regular expression
- SYNOPSIS
`grep pattern filename`
- Searches the text that matches the given PATTERN from FILENAME. If no FILE
NAME is specified then it searches through standard input. Output will be the lines that match the pattern.
- The grep filter searches a file for a particular pattern of characters, and displays all lines that contain that pattern. The pattern that is searched in the file is referred to as the regular expression (grep stands for global search for regular expression and print out). 

`grep -i “search” file`
- case insensitive
`grep -c “search” file`
- count numbers
`grep -l “search” *`
-  displays filename
`grep -R “search” foldername`
- search text in folders
`grep -v ‘term’ filename`
To display without this term
`grep -n “term” file`
To display the term find number

# Wc - word count
- SYNOPSIS
`wc [OPTION]... [FILE]...`
## DESCRIPTION
- It is used to find out number of lines, word count, byte and characters count in the files specified in the file arguments.
`Line(-l)`
`word(-w)`
`byte(-c)`

# Multiple Command Executions
- You can run/ execute multiple commands in 1 line.
- using 3 methods:
      * And ( && )
      * Or ( || ) 
      * Pipeing( | )

# AND ( && )
- It works like if you put an "Enter" after one command and another command starts executing.
- Example : `ls -ltr /home/user && rm –rf /*`
- This means, first ls -ltr /home/user will be executed and only if it's successful then rm –rf /* will be executed.
- Here, ls -ltr /home/user lists all the details of a directory but
before doing so, it executes successfully only if the listing is successful.
- On AND operation All commands you entered will be executed. If both are working without error.

# OR ( || )
- This operator allows us to do something when the first fails.
- Example : `ls -ltr /home/user || echo “Directory not found.”`
- In this example, ls -ltr /home/user tries to list the contents of /home/user. But if it doesn't exist or cannot access then it goes on to the
If it fails then it prints “Directory not found”.
- On OR operation the command will be executed. If it have error or not.

# Piping ( | )
- On pipe, will help you run commands by using the output of the 1st command as the input for the next one.