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
```
mkdir %userprofile%\Desktop\MyLab
```
![444634285-80370d59-0fee-4bd3-8c8d-75579ea43f9b](https://github.com/user-attachments/assets/cb58f6af-92a0-420e-bcfc-af87a9d12a4d)


## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```


![444634434-35039e63-542e-406a-a069-0c354690f62d](https://github.com/user-attachments/assets/3ba9e0cf-820c-4d2e-afda-de9c2599ca86)

![444634487-212e2ccf-0e2e-49e0-8c37-9762f0bd38d5](https://github.com/user-attachments/assets/6b112cfe-c797-462b-b2b5-311d587bd014)


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![444634695-ca7e36bd-0027-43a9-913d-57176ea59df2](https://github.com/user-attachments/assets/d5f871f9-a16c-4306-aabd-c07d3c9eee7f)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![444634913-1aa3e077-5820-477e-b05c-bac217f007d5](https://github.com/user-attachments/assets/24321306-f598-49ce-b054-a96e1ef784fe)

![444635001-bf0c292e-7677-49dc-9dc3-09db0766a3df](https://github.com/user-attachments/assets/b872ee50-09e4-475c-bdaf-6100096be65a)


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![444635197-13d10e67-7ecf-477d-819a-f8606fb2b4c9](https://github.com/user-attachments/assets/c8c940aa-dc2a-417f-a8ef-5fd6980b61e0)

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
![444635643-fafecf65-151a-4219-956d-712d7b07c092](https://github.com/user-attachments/assets/ed8933c3-01f0-40c4-9dfd-88e049c0de4b)

# RESULT:
The commands/batch files are executed successfully.

