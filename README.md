# Ex08 Windows-basic-commands-batchscript
# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
%userprofile%\Desktop\MyLab
```
```
saivishal@Saivishal-laptop:~$ mkdir %nisha%\Desktop\MyLab
```
## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
%userprofile%\Desktop\MyLab
```
```
saivishal@Saivishal-laptop:~$ cd %nisha%\Desktop\MyLab
saivishal@Saivishal-laptop:~/%nisha%DesktopMyLab$ touch MyFile.txt
```
## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
```
saivishal@Saivishal-laptop:~/%nisha%DesktopMyLab$ dir %nisha%\Desktop\MyLab
saivishal@Saivishal-laptop:~/%nisha%DesktopMyLab$ cp MyFile.txt ~/Desktop/Backup/
saivishal@Saivishal-laptop:~/%nisha%DesktopMyLab$ ls MyFile.txt
MyFile.txt
```

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup 
```
```
saivishal@Saivishal-laptop:~/%nisha%DesktopMyLab$ mkdir -p ~/Desktop/Backup
saivishal@Saivishal-laptop:~/%nisha%DesktopMyLab$ file ~/Desktop/Backup
saivishal@Saivishal-laptop:~/%nisha%DesktopMyLab$ ls ~/Desktop/MyLab
saivishal@Saivishal-laptop:~/%nisha%DesktopMyLab$ ls ~/Desktop
MyLab
```


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
```
saivishal@Saivishal-laptop:~/%nisha%DesktopMyLab$ mv ~/Desktop/MyLab ~/Documents/
saivishal@Saivishal:~/%nisha%DesktopMyLab$ ls
%saivishal%DesktopBackup  %nisha%Documents
```


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT:
```
saivishal@Saivishal-laptop:~$ cd ~/Desktop
saivishal@Saivishal:~/Desktop$ nano BackupScript.bat
saivishal@Saivishal:~/Desktop$ nano BackupScript.bat
saivishal@Saivishal-laptop:
```

# RESULT:
The commands/batch files are executed successfully.

