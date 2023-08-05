# Automated File Mover
This program automates file management by effortlessly moving files from one directory to another, as well as searching through a directory locating specific extensions

### Here is a breakdown of the code:
```
import os
```

 
In Python, import os grants access to the "Operating System" module, facilitating interaction with the OS and enabling file and directory operations.

#### To list the files in a certain directory:
```
for file in os.listdir('Directory'):                                                                                                                                         
          print(file)
```
 #### Moving the files:
 ```
for file in os.listdir('INSERT DIRECTORY'):
    if file.endswith('.extension'):
        file_path = os.path.join('INSERT DIRECTORY', file)
        shutil.move(file_path,'INSERT TARGET DIRECTORY')
```

 This code uses Python's os and shutil modules to move all files with a .txt extension from the 'Directory' folder to the 'Target Directory'. It goes through each file in the 'Directory', checks if it ends with .txt, creates the full file path using os.path.join(), and then moves the file to the 'Target Directory' using shutil.move().


