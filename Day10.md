Day 10 - Linux Commands
SOC Analyst Linux Fundamentals

PS - Process Status
Command:
ps aux

Purpose:
Shows all running processes on the computer.

Important Columns:
USER   PID   %CPU   %MEM   COMMAND

USER    = Who started the process
PID     = Process ID (unique number)
COMMAND = What is running

SOC Use Case:
• Unknown programs
• Suspicious scripts
• Crypto miners
• Malware processes

Example:
$ ps aux
USER      PID  %CPU %MEM COMMAND
ubuntu   1234   0.0  0.1 bash
ubuntu   5678   2.1  1.2 firefox

man ls
Command:
man ls

Purpose:
Displays the manual page for ls including usage, options, and examples.

Find
Purpose:
Used to find files and directories.

Useful Symbols:
~ = Home directory
. = Current directory

Examples:

Find all .txt files in current directory:
$ find . -name "*.txt"

Output:
./notes.txt
./soc-lab/example.txt

Find a file anywhere in your home directory:
$ find ~ -name "example.txt"

Output:
/home/ubuntu/Documents/soc-lab/example.txt

Find directories only:
$ find . -type d

Remember:
find     = Search for files/folders
-name    = Search by name
-type f  = Files only
-type d  = Directories only

Grep
Purpose:
Search for keywords or phrases inside files, logs, and documents.

Example:
$ grep error example.txt

Output:
error

Case-insensitive Search:
$ grep -i "error" example.txt

Output:
error
Error
ERROR

Show Line Numbers:
$ grep -n "error" example.txt

Output:
1:error

Netstat
Netstat stands for Network Statistics.

Show all network connections:
$ netstat -an

Show listening TCP and UDP ports:
$ netstat -tuln

Find SSH connections:
$ netstat -ap | grep ssh

SOC Use Case:
• Identify suspicious connections
• Check listening services
• Investigate malware communications

Day 10 Quick Revision
Command	Purpose
ps aux	Show running processes
find	Find files and folders
grep	Search text inside files
netstat -an	Show network connections

<img width="432" height="647" alt="image" src="https://github.com/user-attachments/assets/49b722f5-3397-417f-bb99-841b630356e1" />
