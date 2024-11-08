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
![378696630-9a2cc7df-d480-435a-8f98-4feea6f2a0e9](https://github.com/user-attachments/assets/aed95969-f90a-4317-844c-c4bea417d55d)
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![378696898-a8d269fb-9806-4780-9fc2-7ea10bac4326](https://github.com/user-attachments/assets/c17663ff-e0b3-4c38-abcd-966c9cfa89ab)
![378696925-15d92e5d-5935-4df3-b297-47a74d3afa13](https://github.com/user-attachments/assets/9e5e8b0b-9c5a-4b3b-be90-f3670fe591cb)

List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
![378697436-291694b1-57a1-42b7-8925-ef6cecb12f48](https://github.com/user-attachments/assets/06dc2a59-191d-4494-b27b-6e5e034bae2f)
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
![378697645-cf8c1145-a98d-4290-996b-cb6f834dee13](https://github.com/user-attachments/assets/5de4519f-9784-4dbe-80b9-95b99d6a5cfb)

![378697675-c189166f-5753-4ecd-ae03-77c2b1e71a9a](https://github.com/user-attachments/assets/62c0e320-69f7-4704-a4b0-7b889ae94515)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![378697837-46718950-d9be-4ea8-b9e1-3c058c50ebc9](https://github.com/user-attachments/assets/b0ee4753-1fb4-4f9a-a9e8-7bdc42ea02c0)




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


## OUTPUT
![378698083-06bc777d-4b47-461f-b392-a861609ffa7f](https://github.com/user-attachments/assets/f50ba4ef-34ca-4e4a-981c-f37bf82aa835)

# RESULT:
The commands/batch files are executed successfully.

