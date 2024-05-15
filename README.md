# TryHackMe Journal

## Objective

The objective of this TryHackMe journal is to document my learning journey in cybersecurity, enhancing my understanding through detailed notes, tracking progress, and reflecting on challenges and successes to support continuous growth and skill development.

### Skills Learned

- Advanced understanding of security concepts and practical applications.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- TryHackMe.com
- Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- Telemetry generation tools to create realistic network traffic and attack scenarios.

## Detailed steps can be found below

TryHackMe Journal - Michael Hermann

Entry 1
Room Name: Linux Fundamentals 1
Date Completed: 12/20/2023
Notes During the Room:
Similar to how you have different versions of Windows (7, 8 and 10), there are many different versions/distributions of Linux.


Command --Description
echo --Output any text that we provide
whoami --Find out what user we're currently logged in as!


Command Full Names
ls --listing
cd --change directory
cat --concatenate
pwd --print working directory


Symbol / Operator
& --This operator allows you to run commands in the background of your terminal.
&& --This operator allows you to combine multiple commands together in one line of your terminal.
> --This operator is a redirector - meaning that we can take the output from a command (such as using cat to output a file) and direct it elsewhere.
>> --This operator does the same function of the > operator but appends the output rather than replacing (meaning nothing is overwritten).


Important Takeaways
Linux is an OS, like Windows. There are many different versions of Linux that serve different purposes. 
Linux systems rely more heavily on the command line to do tasks, like navigate the file system. 
Same basic commands while working with files are ls, cd, cat and pwd


Entry 2
Room Name: Linux Fundamentals 2
Date Completed: 04/23/2024
Notes During the Room:
Similar to how you have different versions of Windows (7, 8 and 10), there are many different versions/distributions of Linux.


Command
ssh --Secure Shell - Connect remotely to another device, a protocol between devices in an encrypted form. Using cryptography, any input we send in a human-readable format is encrypted for traveling over a network -- where it is then unencrypted once it reaches the remote machine
ssh user@IPADDRESS > Password
Switches & Flags --Argument provided to command “nano -help” would show all arguments for nano.


Command Names
Man (man pages) --List of all flags/switches for a particular command.

File system commands
Touch --Create file, Mkdir - create folder, cp - copy, mv - move, rm - remove, file - file
su --Switch between available users
Directories --/etc, /var, /root, /home,/tmp


Important Takeaways:
SSH is great for working inside of a server or remote host.
Directories and Remote connections are easy to use with the CLI
Already well versed in linux CLI commands.


Entry 3
Room Name: Linux Fundamentals 3
Date Completed: 04/23/2024
Notes During the Room:


Command
nano --Simple easy to use text editor
vim --My preferred Text editor, many more features and uses CLI
scp --Securely copy a file over SSH from one host to another.
wget/curl --Package installer - Just two of many
Systemctl -Systemctl <arg> <program> (Enable/Start/Stop)
Ctrl + Z OR fg --Sends a program to run in the background/Foreground.


Crontabs
Command and program automation on a schedule. Backing up files using a date/time format.


Important Takeaways:
Scp is super easy to use while your ssh into another machine, and fast.
CLI makes handling linux connections and files easy.


Entry 4
Room Name: Linux Strength Training
Date Completed: 
Notes During the Room:

find /dir/path type f -name = Find files
find /dir/path type d -name = Find directory
find /dir/path type f -size size(c,k,M,G) = Find files by size
find /dir/path type f -user username = Find files by username
find /dir/path type f -group groupname = Find files by group
find /dir/path type f -newermt Date/Time = Find files modified after a specific date
find /dir/path -type f -newermt 1111/22/3 ! -newermt 2222/33/4 = Find files based on date modified 
find /dir/path -type f -newerat 1111/22/3 ! -newerat 2222/33/4 = Find files based on date accessed
grep -iRl /dir/path/Keyword = Find files with a specific keyword
man find = find command manual
mv /file/ /Multiple/files *(all files) /dir/path = Move files to new directory and or rename files
touch, mkdir = Make a file or folder
nano, vim, nvim(preferred) = Open files and folders.
scp = Move folders/files through SSH
./SCRIPT = Run bash/vsh scripts
_______________________________________________________________________________________

Hashing - Super cool usage, stores information in a long string of code that cannot be unhashed. Entering the same information will output the same has hence being able to login on websites without storing text based data.

SHA-256 - Current recommended hash system as MD5 and SHA-1 are considered weak.

Unhashing - programs such as JohntheRipper can be used along with wordlists to attempt to brute force the information. The format can be specified for needed hash algorithms. Can also use hash-identifier or pipe it such as [cat text.txt | hash-identifier].

Base64 - Binary-to-text encoding schemes that represent binary data in an ASCII, some systems rely on a base64 encoding of data for processing while others may not. Use “base64” tool to pipe command cat file.txt | base64 -d [cat file.txt | base64 -d > newtext.txt](new file name).

Encryption - Convert data into an unintelligible code to conceal information, private key to protect data. 
gpg --cipher-algo [encryption type] [encryption method] [file to encrypt]

Decryption - Using the encryption key to make the data legible again.
gpg [file.txt to decrypt]

Cracking Encryption - Brute-force method along with programs such as ‘gpg2john’ which converts the gpg files to hash for johntheripper to compare.
gpg2john [encrypted gpg file] > [filename of the hash you want to create] - creates hash
john wordlist=[location/name of wordlist] --format=gpg [name of hash we just created] - outputs password if found in file.

SQL - Language for storing and manipulating and retrieving data from a database.
Relational databases - Multiple databases that reference each other(Similar to a multi config folder). Each database contains tables of records and each table can consist of multiple columns and rows which store the data in an organized format.
service mysql start/stop - Starts or stops mysql
mysql -u username -p -h 100.10.15.1 = Remote connection
mysql -p password = If set for Auth
mysql -u username -p = Login to mysql
source sql file = Specify database to open
SHOW DATABASES; = Shows all Relational databases
USE database = Chose which database to show.
SHOW TABLE; = Displays selected database tables
DESCRIBE table = view the table structure of individual tables
SELECT * FROM table = Shows ALL data from table


Entry 5
Room Name: Intro to Logs
Date Completed: 
Notes During the Room:




Important Takeaways:



Entry 6
Room Name: Wireshark Basics
Date Completed: 
Notes During the Room:




Important Takeaways:



Entry 7
Room Name: Wireshark 101
Date Completed: 
Notes During the Room:




Important Takeaways:



Entry 8
Room Name: Windows Fundamentals 1
Date Completed: 
Notes During the Room:




Important Takeaways:



Entry 9
Room Name: Windows Fundamentals 2
Date Completed: 
Notes During the Room:




Important Takeaways:



Entry 10
Room Name: Windows Fundamentals 3
Date Completed: 
Notes During the Room:




Important Takeaways:



Entry 11
Room Name: Windows Forensics 1
Date Completed: 
Notes During the Room:




Important Takeaways:



Entry 12
Room Name: Windows Forensics 2
Date Completed: 
Notes During the Room:




Important Takeaways:



Entry 13
Room Name: Intro to Log Analysis
Date Completed: 
Notes During the Room:




Important Takeaways:



Entry 14
Room Name: Splunk Basics
Date Completed: 
Notes During the Room:




Important Takeaways:



Entry 15
Room Name: Incident Handling with Splunk
Date Completed: 
Notes During the Room:




Important Takeaways:



Entry 16
Room Name: Splunk 2
Date Completed: 
Notes During the Room:




Important Takeaways:



Entry 17
Room Name: Splunk 3
Date Completed: 
Notes During the Room:




Important Takeaways:





