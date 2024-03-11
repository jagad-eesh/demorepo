1) sudo su - (switch to the root user)
2) ls / (/ means root) what and all dir are there in the root
https://en.wikipedia.org/wiki/Filesystem_Hierarchy_Standard

3) date: shows the current date and time
4) cal: shows the months's calendar
5)  uptime: show current uptime
6) whoami: who you are logged in as
7) finger: display information about user
8) users/id: shows user information
9) man command: shows manual of command
10)  username: shows your user name
11) who /w: display who is online

 VIEW FILES
 1) ls: directory listing
 2) cat filename: view file content
 3) less: view a file page by page
 4) more: output the content of file
 5) head: output of the first 10 lines of file
 6) tail: output of the last 10 lines of file
 7) page: display file page by page

 CREATE AND DELETE FILE/DIRECTORY
 1) touch: creates a 0 bite file
 2) cat>filename: create file and allow to write
 3) nano : create a file if file name is doesn't exist (control+o, press enter, 
   control+x)
 4) vi : create a file if file name is doesn't exist
 5) rm : remove a file
 6) mkdir: create a directory
 7) rmdir: remove a empty directory
 8) rm -rf: remove a directory

Manging files or Directories
1) cp: copy a file
2) mv: move a file
3) find: find a file
4) grep: search for a pattern a file
5) cd: switch between directories
6) diff: find content difference in 2 files
7) sed: search and replace particular pattern
8) chmod: change file permission
9) chown: change owner ship of file
10) file: show what kind of file it is

find command
  find command is used to find the files or directorie's path, it is exactly like the find option in windows where you can search for a file
     syntax: find / -option filename
        -name: for searching a file with its name
        -user: for files whose owner is a particular user
        -group:  for files belonging to particular group
        
grep command
  grep stands for global regular expression print.
  it is used to pick out the required expression from the file and print the 
   output.
     syntax: grep <patron> filename
