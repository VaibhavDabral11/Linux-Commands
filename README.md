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

 mv filename foldername [ move file from one folder to another folder]
```
9. Display the content of file in terminal by using this  folling command .

```@ruby
 cat filename 
```

10. Copy any file using this commands .

```@ruby
 cp filename
```

11. print the file tree in terminal using this commads . 

```@ruby
 tree filename
```
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

17. Shutdown in linux :

```@ruby
sudo shutdown -h now
```
   set time for shutdown 

```@ruby
sudo shutdown -h 22:30
```
18.  if-else and else-if statement in linux :

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
fi

```
-f : find

for executing this file ```chmod +x scriptname.sh ``` for enable executing rights 
then execute using this commands ``` ./scriptname.sh ```

19. For checking dir rights use this ``` ll ``` commands . 
