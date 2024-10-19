# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

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
mkdir %userprofile%\Desktop\MyLab

![Screenshot 2024-10-18 160446](https://github.com/user-attachments/assets/828dbb9e-699e-4a69-83f5-213fc5134e7e)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab


![image](https://github.com/user-attachments/assets/89d4774b-d47c-4964-819b-9e74751cf9cb)



![image](https://github.com/user-attachments/assets/8afeddef-6cb9-4ac6-82d1-b37ea10510ef)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab


![image](https://github.com/user-attachments/assets/88377d5b-63af-42a8-bf1b-c78872ce4e6b)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup


![image](https://github.com/user-attachments/assets/3851e3c1-f59d-4359-81b7-f84098fabd7f)


![image](https://github.com/user-attachments/assets/8d6fe70e-509f-45e8-b578-6bc5cb8f7867)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/user-attachments/assets/e01c3ceb-c361-4170-8f12-ecb0ae456776)



## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
~~~

Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.

~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
~~~


## OUTPUT


![image](https://github.com/user-attachments/assets/70b1b765-2e0a-444a-9ccd-30c6ec09a98b)




# RESULT:
The commands/batch files are executed successfully.

