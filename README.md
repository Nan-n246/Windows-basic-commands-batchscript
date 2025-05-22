# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file . Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "my-folder"

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-22 101908](https://github.com/user-attachments/assets/8c630ea1-c5ac-49df-8ec3-6acc0c2301df)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-22 102039](https://github.com/user-attachments/assets/541a9fa1-c63e-4ada-959d-801965214f85)

type nul > MyFile.txt

![Screenshot 2025-05-22 102150](https://github.com/user-attachments/assets/465de4c6-8fdb-4fcc-8266-fb6714010df7)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-22 102304](https://github.com/user-attachments/assets/f1318bf3-9abd-4b65-aaad-eb05e405d219)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![Screenshot 2025-05-22 102400](https://github.com/user-attachments/assets/6899ed88-d0f7-4245-a7ac-6776e5492c5a)

copy MyFile.txt %userprofile%\Desktop\Backup
![Screenshot 2025-05-22 102437](https://github.com/user-attachments/assets/c0f72d8c-01eb-40d2-8a84-598c12a31b5a)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
```
move MyLab Documents
![Screenshot 2025-05-22 102539](https://github.com/user-attachments/assets/691cc2d1-6b1b-4be3-9cf9-787a0424e689)


## Exercise 2: Advanced Batch Scripting
Create a batch file named on the desktop. The batch file need to have a variable assigned with a desired name for ex. name="John" and display as "Hello, John".

## command
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

## OUTPUT

![Screenshot 2025-05-22 102815](https://github.com/user-attachments/assets/0281d22f-0e58-48df-ba68-c551b320c051)

## command
```
  @echo off
  mkdir %userprofile%\Desktop\DocBackup
  copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
  del %userprofile%\Documents\*.docx
  echo Backup and deletion completed successfully!
```

## OUTPUT

![Screenshot 2025-05-22 102927](https://github.com/user-attachments/assets/943b47bd-2a75-4408-877e-c1936b6fe6a3)


# RESULT:
The commands/batch files are executed successfully.

