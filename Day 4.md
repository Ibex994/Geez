# Linux File Hierarchy
- Linux/Unix have a special file system than windows.
- file system is a directory structure that the OS uses.

# System Files
- system files are files used by the software(OS).
- **Windows**: System files appear under **Local disk C:**.
	- **Linux**: System files appear under the **root directory(/)**.

## File Structure In Details
1. ### /(root)
	* Every single file amd directory starts from root directory.
	* the only root user has the right to write under this directory.
	* /root is the root user's home directory, which is not the same as `/`.
			
2. ### bin -Binary excutables
	* Essential command binaries that needs to be available in single-user model;for all users.
		- e.g) cat,ls,cp,pwd
		
3. ### /boot- Boot loder files
	* kernal initrd, vmlinux,grub files are located under **/boot**.
		- Exmaple: initrd.img-2.6.32-24-generic,
		 vmlinux-2.6.32-24-generic
		 
4. ### /dev- Essential Device Files
	* These include terminal device, usb or any device attached to the system.
		- Example:/dev/tty1,/dev/usbmon0

5. ### /etc-et cetera
	- containes configuration files required by all programs.
	- This also contains startup and shutdwon shell scripts used to start/stop individual programs.
		- Example: /etc/resolve.conf, 
			/etc/logrotate.conf
	
6. ### /home-Home directory
	- Home directories for all users to store their persoal files.
		- Example:/home/nathan,/home/rexdar

7. ### /lib-Libraries essential for the binaries in /bin and /sbin
	- Libraries filenames are either **ID** or **lib** *.so.*
		- Example: Id-2.11.1.so,
			libncurses.so.5.7

8. ### /media-Mount points for removable media such as CD-ROMS
	- Temporary mount directory for removable device.
		- Example:/media/cdrom for CD-ROM;
				/media/floopy for floppy drives;
				/media/cdrecorder for CD writer

9. ### /mnt-Temporary mounted files
	- Temporary mount directory where sys admins can mount file systems.

10. ### /opt-Optional application software pakages
	- Contains add-on applications from individual vendors. 
	- Add-on applications should be installed under either **/opt/** or **/opt/ sub-directory**.

11. ### /sbin-Essential system binaries 
	- Just like /bin, /sbin also contains binary executables. 
	- The linux commands located under this directory are used typically by system administrator, for system maintenance purpose.

12. ### /temp-Temporary files
	- Directories that contains temporary files created by system and users.
	- Files under this directories are **deleted** when the system is rebooted.

13. ### /usr - User Utilities 
	- Contains binaries, libraries, documentation, and source-code for second level programs. 
	- /usr/bin contains binary files for user programs. If you can’t find a user binary under /bin, look under /usr/bin. 
		 - Example: at, awk, cc, less, scp 
	- /usr/sbin contains binary files for system administrators. If you can’t find a system binary under /sbin, look under /usr/sbin. 
		- Example: atd, cron, sshd, useradd, userdel 
	- /usr/lib contains libraries for /usr/bin and /usr/sbin 
	- /usr/src holds the Linux kernel sources, header-files and documentation.

# Text Editors
- Programs that used for text processing.
- Linux command line text editor.
	- VIM 
	- Nano
	- Emacs
	- Neovim
	- .........
- Linux Graphical Text Editor
	- sublime
	- vs code
	- Gedit
	- pluma
	- ...........
### VIM 
- Before vi the primary editor used on Unix was the line editor  
- User was able to see/edit only one line of the text at a time 
- Then then vi editor improved and developed VIM. ( VI iMproved) 
- The ViM Editor is a 
	- very powerful
	- but at the same time it is cryptic 
	- It is hard to learn, specially for windows users 
- It have mainly to modes 
	- **Command mode** -> where you can do commands 
	- **Input mode** -> where you can write.

- Syntax
	- `vim yourfilename`

- Vim is by default on **command mode** when you open it.
- To get on **insert mode** you have to press `i`.
- To get back to command mode 
you press `esc`.
- Inside Command mode you can
	- Save: Type `:w` + enter
	- Quit: Type`:q` + enter
	- Force Quit & Save: Type `:wq!` + enter Force = !
	- Undo: Type `:undo` + enter
Or ``:u````
	- Execute bash commands:Type
`:%!yourcommand`
NB: **THERE IS NO SPACE BETWEEN THEM**

### NANO
- The GNU nano text editor is a user-friendly, free and open-source text editor that usually comes pre-installed in modern Linux systems. 

#### Starting nano
-Syntax
- `nano filename` Then start typing.

#### Saving Exiting & Undo_redo
	- Ctrl + S - save
	- Alt + U - Undo
	- Alt + E - Redo
	- Ctrl + X - Exit
#### Paste,Copy & paste all over the linux is

	- Ctrl + shift + C - copy
	- Ctrl + shift + X - Cut
	- Ctrl + shift + V - Paste 
- **The ^ is equal to ‘Ctrl’**  
#### Linux User Management
- On Computer system, person who uses the computer is called “user”
- Every Users have Group.
- Users have their own file & applications.
- To know our name on linux ->  `whoami`
- Those users have power/privilege.
- On linux  there's 2 kinds users.
	- Root  id = 0
	- Normal User id start with 1-999
- The root user have the power to do everything on linux , 
but if users want to have a root access they add sudo in front of the command .

		`sudo YourCommand`
- **SUDO = Superuser do  ,  used to pass permission denied**

#### Creating Users
- On linux, to create users you can use the following commands
	- Useradd -> simple 
	- Adduser   -> Detailed
- Useradd command
	- sudo useradd username
- Adduser command
	- sudo adduser username
- The User files are stored inside /etc/passwd
- The User password are stored inside /etc/shadow
- When you create a user **it creates a group with that name.**

#### Checking /etc/passwd
- This happened what shall i do?
	- `cat/etc/shadow`
	- `id`

#### To access root user
- Command `sudo su`

