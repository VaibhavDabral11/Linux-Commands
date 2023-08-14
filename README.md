# Linux-Commands

1. This command is use to clear the data in the terminal .                                                                        *files/dirs

```@ruby
 clear
```

2. This commands is use to print the parent files in the terminal .

```@ruby
 ls
```

3. This commands is use to print both parent and  hidden folders in the terminal .

```@ruby
 ls -a
```

4. This commands is use to print both parent and child files in the terminal . 

```@ruby
 ls -R
```

5. This commands is use to displays the contents of the directory in reverse order .

```@ruby
 ls -r
```
6. This commands is use for basic shell scripting. [vim]

```@ruby
 vim file_name 

press i for insert 
press Esc for escape the editer.
write :q for quit and press Enter .
write :w for save and press Enter .
```
[Indetail](https://www.educba.com/vim-command-in-linux/)

7. These folling commands for deleting files and folders .

-To delete the file named myfile, type the following:

```@ruby
 rm myfile
 
 rm -rf .git*
```
-To delete all the files in the mydir directory, one by one, type the following:

```@ruby
 rm -i mydir/*
```
- To the folders named myfolders, type the following:

```@ruby
 rmdir myfolders
```
[Indetails](https://www.hostinger.in/tutorials/how-to-remove-files-and-folders-using-linux-command-line/#:~:text=Folders%20in%20Linux%3F-,How%20to%20Remove%20a%20Directory%20in%20Linux,to%20remove%20non%2Dempty%20directories.)

8. For rename and also move the files from one folder to anther folder files use this following  command .

```@ruby
 mv filename newFilenName [rename]

 mv foldername foldername [ move file from one folder to another folder]
```
9. Display the content of file in terminal by using this  folling command .

```@ruby
 cat filename 
```

10. Copy any file using this commands .

```@ruby
 cp filename/foldername
```

11. print the file tree in terminal using this commads . 

```@ruby
 tree filename
```

To list the directory structure in Linux while excluding the "node_modules" directory, you can use the "tree" command along with the "--exclude" option. The "tree" command is not installed by default on some systems, so you might need to install it first. Here's how you can list the directory structure excluding "filename":
```@ruby
tree --prune -I 'filename'
```
Let me explain the options used in this command:

--prune: This option prevents the specified directory (in this case, "filename") from being displayed in the output.

-I 'filename': This option tells tree to exclude directories matching the given pattern (in this case, "filename").

12. [ How to check system specs in Linux Commands . ](https://github.com/VaibhavDabral11/linux-specs-check/blob/main/README.md) 

13. [How to check the storage , ram and gpu usage of any files and folder Using Linus Commands . ](https://github.com/VaibhavDabral11/Linus-Folder-Storage/blob/main/README.md) 

14. [how to active and close the virtual environments in linux .](https://github.com/VaibhavDabral11/linux1/blob/main/README.md)

15. copy files and folders :
```@ruby
files :   cp floder2/f3.txt  folder/   [condition: both folder present in same folder]   
          cp  path1 path2
```
```@ruby
folders :    cp -r folder/f1  folder1/    [condition: both folder present in same folder]
```
16. move files and folders :
```@ruby
files :   mv floder2/f3.txt  folder/   [condition: both folder present in same folder    
          mv  path1 path2
```
```@ruby
folders :    mv -r folder/f1  folder1/    [condition: both folder present in same folder]
```

17. Shutdown in linux :-

```@ruby
sudo shutdown -h now
```
   set time for shutdown 

```@ruby
sudo shutdown -h 22:30
```
18.  if-else and else-if statement in linux :-

```@ruby
#!/bin/bash

echo "Enter a number: "
read num 

if [ $num -gt 0 ]
then   
   echo "number is Positive "

elif [ $num -lt 0 ]
then 
   echo "number is negative "

else 
   echo "number is zero"

fi   
```
-gt : greater than
-lt : less than
```@ruby
#!/bin/bash

# Check if a file exists
if [ -f "/path/to/file.txt" ]
then
    echo "File exists"
else
    echo "File does not exist"

fips aux | grep code
```
-f : find

for executing this file ```chmod +x scriptname.sh ``` for enable executing rights 
then execute using this commands ``` ./scriptname.sh ```

19. For checking dir rights use this ``` ll ``` commands :-
 
21. For finding any file and a folder use these commands given bellow :-
```
find . -name "example.txt" 
find . -name "folderName"
```
22. Kill process in Linux.
    1. Firstly list process uaing given command bellow :
       ```@ruby
        ps aux | grep code
       ```
    2. Then kill the process using this command given bellow :
       ```@ruby
        pkill proces_id
       ```
23. This is  interactive process viewer and system monitor build for linux use given bellow command :
```@ruby
htop    
```
24. This given bellow command is use to  change the permissions of a file or directory.
```@ruby
# The first digit represents the owner of the file/directory
# The second digit represents the group that the file/directory belongs to
# The third digit represents all other users
# 0 (no permission)
# 1 (execute only)
# 2 (write only)
# 3 (write and execute)
# 4 (read only)
# 5 (read and execute)
# 6 (read and write)
# 7 (read, write, and execute)

chmod 700 file.txt

```
25. change the ownership of the die using this commands given bellow.
```@ruby
chown new_owner example.txt
```
26. This given bellow commands is use to create or extract compressed archive files.
```@ruby
'tar'
# x: extract files from an archive
# t: list the contents of an archive
# r: append files to an existing archive
# z: use gzip compression
# j: use bzip2 compression
# cf: create file
#xf: extract file
tar cf archive.tar file1 file2 file3
```
27. For compress files in linux sue this given bellow command.
```@ruby
gzip file.txt
``` 
29. For  decompress compressed files in linux sue this given bellow command.
```@ruby
gunzip file.txt.gz
```
30. connect to a remote server securely using this command.
```@ruby
ssh username@server_address
```
31. securely copy files between systems in linux.
```@ruby
scp filename.txt machine_ip folder_where_this_file_is_located
like this : scp myfile.txt user@remotehost:/home/user/
```
32. check ping of any site by this command
```@ruby
 ping www.google.com
```
33. display or configure network interfaces using this command
```@ruby
netstat
```
34. view or configure network routing tables using this command
```@ruby
route [options] [add/delete/show]
```
35. display system resource usage and processes using this command
```@ruby
top
```
36. control system services and settings using this command
```@ruby
# Start the nginx service
systemctl start nginx control system services

# Check the status of the nginx service
systemctl status nginx

# Stop the nginx service
systemctl stop nginx

```
37. control system services
```@ruby
service apache2 start
```
38.  add a new user to the system
```@ruby
useradd harry
```su john
39.  change the password for a user
```@ruby
passwd harry
```
40.  delete a user from the system
```@ruby
 userdel harry
```
41. switch user to become another user
```@ruby
su john
 ```
42. execute a command as another user or with elevated privileges
```@ruby
sudo
```
43. display system uptime and load average
```@ruby
uptime
```
44. display disk space usage
```@ruby
df
```
45. display disk usage by file or directory
```@ruby
du
```
46. mount a file system
```@ruby
sudo mount /dev/sdb1 /mnt/usb
```
47. unmount a file system
```@ruby
sudo umount /mnt/usb
```
48. display or set the system date and time
```@ruby
date
 ```
50. display the current user name
```@ruby
whoami
```
51. displays all the information about user
```@ruby
finger filename
```
52. display system information
```@ruby
uname
uname -a
```
53. redirect output to both a file and the console
```@ruby
$ ls | tee file.txt
```
54. locate any file on the system
```@ruby
locate file.txt
```
55. sort lines of text in a file or input
```@ruby
cat file.txt
banana
orange
apple
sort file.txt
apple
banana
orange
```
56. remove duplicate lines from a file or input
```@ruby
cat file.txt
apple
orange
banana
apple
banana
uniq file.txt
apple
orange
banana
```
57. display the first/last few lines of a file or input
```@ruby
#display first 10 lines
head file.txt

#display last 10 lines
tail file.txt
```
58 print the last two elements 
```@ruby 
tail -2f filename.txt
```
59. find process using this command
```@ruby
ps -ef | grep sbin
```     
60. check history using this command
```@ruby
history
```
61. Text Editer in linux
```@ruby
nano filename.txt
```

    
