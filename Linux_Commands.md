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

USER MANAGEMENT
# In linux there are three types of users
# Super or Root user: User is the most powerful user. He is the adminstrator user.
# Normal User: Normal Users are the users created by root user

   TYPE              EXAMPLE     HOME DIRECTORY     SHELL
   super user        root         /root              /bin/bash
   system user       ftp,ssh,apache  /var/ftp, etc    /sbin/nologin
   Normal user       visitor,ec2-user /home/username   /bin/bash

/etc/passwd this file contain all the users related information

# Software Management
  yum is the primary tool for getting,installing, deleting, quering, and managing REDHAT Enterprise Linux RPM Software packages from official Redhat software repositories , as well other third party repositories.
 #  COMMANDS
  1) yum install <package name>
  2) yum remove <package name>
  3) yum update <package name>
  4) yum info <package name>
  5)  yum list available
  6)  yum list installed

  # Archiving files or directories
   gzip: Create a compressed file
   gunzip: unzip a file
   tar: to extract a file
    1)  gzip file1
    2)  gunzip file1.gz
    3)  yum install zip -y
     4)  zip file1.zip file1
    usually zip and gzip work on files not directories, for dir we are use tar command
    5)  tar -cvf dir1.tar dir1
    6)  rm -rf dir1
    7)  tar -xvf dir1.tar
    8)  gzip dir1.tar
    9)  tar -xvzf apache-tomcat-9.0.86.tar.gz
# Copy files between servers
 Windows to linux : mobaxterm or winscp
 Linux to Linux
 SCP(SECURE COPY)is command line utility that allows you to securely copy files and directories between two system
 # scp source_file_name username@destination_host:destination_folder
 EXAMPLE
 1) scp file1 root@10.20.30.40:/tmp
 2) scp file1 root@10.20.30.40:/tmp /home/ec2-user
 3)  scp test@172.31.15.95:/home/test/file2 /home/ec2-user


