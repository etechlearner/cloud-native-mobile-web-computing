## User Role and Sudo
- Package Install Command 
```` 
$ sudo apt-get install package 
```` 
Note : Normal user not able to install or system changes you must switch user to root or start command with **sudo**  
## Command Completion and Shortcut
- when we typing a command in linux use most common and use full commands 
````
# Tab key  : for autocomplete the avalible possiblity
# Ctrl + E key  : for move the cursor start form end 
# Ctrl + A key  : for move the cursor end form start 
# Arrow up key  : for show previous executed command
# Arrow down key  : for show last executed command
````

## File Directory and wirte and overwite
- File Create
````
$ touch file.txt
````
- View file content 
````
$ cat file.txt
````
   - **File Write** (<<EOT >>  EOT) Append the text into new line at the end to file.txt 
````
$   cat <<EOT >> file.txt
    line 1
    line 2
    EOT
````
````
$   cat << EOF > file.txt
    echo "$PWD" # echo the current path
    EOF
````
- Echo Editor  
   - **Double Arrow** (>>) Append the text into new line at the end to file.txt 
````
$ echo "world" >> file.txt
````
   - **Single Arrow** (>>) Override all the text into The file.txt 
````
$ echo "world" > file.txt
````
   - **Single Arrow** (>) with  Append the text into new line at the end to file.txt
````
$ echo 'task goes here' | cat - file.txt > temp && mv temp file.txt
````        
   - **Create Variable** on terminal variable value  
````
$ url='http://www.whitehouse.gov'
````
   - **Print** with  print value of terminal variable value  
````
$ echo $url
````
- List file and directory  
   - **Simple List**
````
$ ls
````
   - **Write all directory structure into file **
````
$ ls > file.txt
````
   - **Append all directory structure into file **
````
$ ls >> file.txt
````
   - **List all files and directory with hidden files and directory  **
````
$ ls -la
````
   - **List all files and directory with grace full view + file and directory Permission **
````
$ ls -l
````
   - **List all files and directory log save in any  file  **
````
$ ls -l | less
````
   - **List all files and directory which are Recently updated by time   **
````
$ ls -lt | head
````
   - **List all files and directory which are Oldest updated by time   **
````
$ ls -lt | tail
````
## Editor
   - **VI editor** native linux editor
````
$ sudo vi file.txt
````
   - **VI editor** after open file in editor press "i" to enable editing
````
# press i
````
   - **VI editor** after changes to save file short key esc ->  shift + ZZ
````
# ZZ
````
   - **VI editor** cut single line short key  esc -> dd
````
# dd
````
   - **VI editor** cut number of line short key  esc -> 2dd
````
# 2dd
````
   - **VI editor** copy single line short key  esc -> yy
````
# yy
````
   - **VI editor** copy number of line short key  esc -> 2yy
````
# 2yy
````
   - **VI editor** paste short key  esc -> p
````
# p
````
   - **VI editor** replace single character   esc -> r
````
# r
````
   - **VI editor** replace character till hit character  esc -> R
````
# R
````
   - **VI editor** search forword first work start capital   esc -> /Test
````
# /Test
````
   - **VI editor** search backword first work start capital   esc -> /Test
````
# /test
````
   - **VI editor** undo changes esc -> u
````
# u
````
   - **VI editor** redo changes esc -> Ctrl + r
````
# Ctrl + r
````
   - **VI editor** after changes to save file  press esc -> shift + colon -> wq
````
# :wq
````
   - **VI editor** after changes to do not save file  press esc -> shift + colon -> aq
````
# :qa!
````
## Scripting
   - **bash script** first line
````
# #!/bin/bash
````
   - **bash script** create variable
````
$ data=value
````
   - **bash script** get param variable value
````
$ $1
````
## File Permissions
   - **permission** permissions as name and value
````
# 0  : no permissions
# 1  : executable permissions 
# 2  : write permissions 
# 4  : read permission
````
   - **permission** Classes check ls -l
````
# -rw-r--r-- 1 tahir-app tahir-app      14 Apr  7 11:58  fiel.txt
# --- (file owner) --- (user Group) --- (other user) user(tahir) group(admin)
````
   - **permission** assign permission to any class
````
$ sudo chmod -R 777 file.txt
````   
   - **permission** change file owner 
````
$ sudo chown -R username:group directory
````   
## General Commands
   - **gerneral commands** check when my system is running 
````
$ uptime
````   
   - **gerneral commands** check system name 
````
$ uname
````   
   - **gerneral commands** check system name and release version 
````
$ uname -srv
````   
   - **gerneral commands** to check command help 
````
$ man ls 
````   
   - **gerneral commands** change directory to home
````
$ cd ~ 
$ cd ./home
$ cd ../ 
````   
   - **gerneral commands** to check directory current path
````
$ pwd
````   
   - **gerneral commands** to check hostname or node name
````
$ hostname 
````   
   - **gerneral commands** to check hostname default ip
````
$ hostname  -i
````   
   - **gerneral commands** to check current date
````
$ date
````   
   - **gerneral commands** to check calender
````
$ cal
```` 
   - **gerneral commands** which user is currently login in system
````
$ w
````   
## Copy Move and Remove
   - **copy move** copy to and form
````
$ sudo cp -R ~/myfolder  ~/Desktop/
````
   - **copy move** copy to and form
````
$ sudo mv -R ~/myfolder  ~/Desktop/
````
## Search Using Command Line
   - **search** search file form any where
````
$ find ~/Desktop/Workspace -name "mytext*" 
````
## CPU information and Hard Disk
   - **cpu info** system cpu info and system bits
````
$ uname -a
$ uname -p
```` 
   - **cpu info** system cpu architecture info 
````
$ lscpu
$ cat /proc/cpuinfo
```` 
   - **cpu info** system use and avalible space  
````
$ df
```` 
   - **cpu info** system use and avalible space  with unit
````
$ df -h
```` 
   - **cpu info** current directory use and avalible space 
````
$ du 
```` 
   - **cpu info** current directory use and avalible space size with unit
````
$ du -s -h
```` 
## Install Software Package Manager
   - **software install** package intallation
````
$ sudo apt install cpuid
```` 
   - **software install** package remove
````
$ sudo apt remove cpuid
```` 
   - **software install** package search
````
$ sudo apt-cache search pithon
````
   - **software install** package update and upgrade
````
$ sudo apt-get update && apt-get upgrade
```` 
   - **software install** package remove unuse 
````
$ sudo apt-get autoremove
```` 
## Create Custom Commands
   - **custom commands** make custom commonds 
````
$ alias cf="touch cf.txt"
````
   - **custom commands** make custom commonds create file without extention
````
$ sudo vi /usr/bin/cf
````
   - **custom commands** remove custom commonds 
````
$ unalias createFile
```` 
## User Management
   - **user management** create user with add directory on home 
````
$ sudo useradd tahir -m 
```` 
   - **user management** set user password 
````
$ sudo passwd tahir 
```` 
   - **user management** delete user with add directory on home 
````
$ sudo userdel tahir -r 
```` 
   - **user management** View the Groups a User Account is Assigned To 
````
$ groups
```` 
   - **user management** create group  
````
$ sudo groupadd mynewgroup
```` 
   - **user management** Add an Existing User Account to a Group 
````
$ sudo usermod -a -G examplegroup exampleusername
```` 
   - **user management** Add the user geek to the group sudo , use the following command
````
$ sudo usermod -a -G sudo geek
```` 
   - **user management** Change a User’s Primary Group
````
$ sudo usermod -g groupname username
```` 
   - **user management** show user and groups id
````
$ id
````
   - **user management** get all user by username
````
$ id user-name
````  
   - **user management** get all groups by username
````
$ groups user-name
```` 
   - **user management** create use with custom group name
````
$ useradd -G examplegroup exampleusername
```` 
   - **user management** add user to multi groups
````
$ usermod -a -G group1,group2,group3 exampleusername
```` 
   - **user management** get all associated groups
````
$ getent group
```` 








## Essentail Commands
   - **essentail commands** create user with add directory on home 
````
$ sudo useradd tahir -m 
```` 
   - **essentail commands** get command info  
````
$ info cat 
```` 
   - **essentail commands** where should execute the command 
````
$ type man 
```` 
   - **essentail commands** where is file and command path  
````
$ whereis man 
```` 
   - **essentail commands** where is execute file  path variable 
````
$ which man 
```` 
   - **essentail commands** see backgroud process
````
$ bg 
```` 
   - **essentail commands** check free space with unit
````
$ free -h
```` 
   - **essentail commands** check processes
````
$ ps
```` 
   - **essentail commands** kill processes
````
$ kill process id
````
   - **essentail commands** show all runing processes
````
$ top
````
   - **essentail commands** system restart
````
$ reboot
````
   - **essentail commands** system shutdown
````
$ shutdown
````








