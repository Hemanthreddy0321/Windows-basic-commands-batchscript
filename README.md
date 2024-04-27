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
```
mkdir %userprofile%\Desktop\MyLab
```

![image](https://github.com/Hemanthreddy0321/Windows-basic-commands-batchscript/assets/150005937/36cf0843-ad33-4303-958a-dda5a716a466)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```

![image](https://github.com/Hemanthreddy0321/Windows-basic-commands-batchscript/assets/150005937/ba198d0f-360a-4278-98a4-dac8e12a9393)


![image](https://github.com/Hemanthreddy0321/Windows-basic-commands-batchscript/assets/150005937/4f27d0cf-db4e-4fe6-b7a2-86c61f5d0fd4)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```

![image](https://github.com/Hemanthreddy0321/Windows-basic-commands-batchscript/assets/150005937/a308a9a7-c695-461f-91c6-fd8834d68ff3)


copy MyFile.txt %userprofile%\Desktop\Backup

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```

![image](https://github.com/Hemanthreddy0321/Windows-basic-commands-batchscript/assets/150005937/acbd5b11-ff58-42b8-b1e3-e849dcaca240)


![image](https://github.com/Hemanthreddy0321/Windows-basic-commands-batchscript/assets/150005937/2c2af1f6-cf2c-4775-b934-d94be0c6941d)



Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```

![image](https://github.com/Hemanthreddy0321/Windows-basic-commands-batchscript/assets/150005937/769b945d-5444-4961-920c-4c9118646f57)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```






## OUTPUT


![image](https://github.com/Hemanthreddy0321/Windows-basic-commands-batchscript/assets/150005937/da341298-7dcc-48e5-9609-2bd9b1119852)





# RESULT:
The commands/batch files are executed successfully.

