### ```sudo apt install PackageName```
- Installs a package.
- Example: ```sudo apt install tcpdump```

---

### ```sudo apt remove PackageName```
- Uninstalls a package.
- Example: ```sudo apt remove tcpdump```

---

### ```apt list --installed```
- Shows installed applications.

---

### ```echo```
- Generates output in the shell.
- Examples: 
  - ```echo "Hello World"```
  - ```echo "Hello" > file.txt``` overwrites the existing file with the new content.
  - ```echo "Hello" >> file.txt``` adds the new content to the end of the existing file.
  

---

### ```expr```
- Performs basic calculations.
- Example: ```expr 5 + 5```

---

### ```clear```
- Clears the shell window.

---

### ```pwd```
- Prints the working directory onto the screen.

---

### ```ls```
- Displays the names of files and directories in the current working directory.
- Examples:
  - ```ls /home/analyst```
  - ```ls -l /home/analyst``` Displays the permissions to files and directories.
  - ```ls -a /home/analyst``` Displays hidden files.

---

### ```cd```
- Navigates between directories.
- You can use ```cd ..``` to go up one level in the file structure.

---

### ```clear```
- to clear the shell window.

---

### ```cat```
- Displays the content of a file.

---

### ```head```
- Displays just the beginning of the file, by default 10 lines.
- You can use ```head -n ``` to specify a number of lines, for example: ```head -n 5 log.txt```.

---

### ```tail```
- Displays just the end of the file, by default 10 lines.
- You can use ```tail -n ``` to specify a number of lines, for example: ```tail -n 5 log.txt```.

---

### ```less```
- returns the content of a file one page at a time.
- Some useful shortcuts:
  - Space bar: Move forward one page.
  - b: Move back one page.
  - Down arrow: Move forward one line.
  - Up arrow: Move back one line.
  - q: Quit and return to the previous terminal window.
  

---

### ```grep```
- Searches a specified file and returns all lines in the file containing a specified string.
- Examples: 
  - ```grep hello file.txt```
  - ```ls /home/analyst/reports | grep users```

---

### ```find```
- searches for directories and files that meet specified criteria.
- Examples: 
  - ```find /home/analyst/reports -name "*users*"``` to find file or directory names that contain a specific string (case-sensitive)
  - ```find /home/analyst/reports -iname "*users*"``` to find file or directory names that contain a specific string (not case-sensitive)
  - ```find /home/analyst/reports -mtime -3``` returns all files and directories in the projects directory that have been modified within the past three days. 
  - ```find /home/analyst/reports -mmin -3``` returns all files and directories in the projects directory that have been modified within the past three minutes. 

---

### ```mkdir```
- Creates a new directory.

---

### ```rmdir```
- Removes a directory.

---

### ```touch```
- Creates a new file.

---

### ```nano```
- Creates or Edits a file.

---

### ```rm```
- Removes a file.

---

### ```mv```
- Moves a file or directory to a new location.
- Example: ```mv file.txt /home/analyst/newLocation```

---

### ```cp```
- Copies a file or directory into a new location
- Example: ```cp file.txt /home/analyst/newLocation```

---

### ```chmod```
- Changes permissions on files and directiories.
- Examples: 
  - ```chmod u+w,g+r file.txt``` adds write permission for user, and read permission for group.
  - ```chmod u=w,g=r file.txt``` set exactly write permission for user (removes other permissions), and exactly read permission for group.
  - ```chmod a+a``` adds all permissions for all users, groups, and others.
  - ```chmod ugo+r``` adds read permission for all users, groups, and others.

---

### ```sudo chown```
- changes ownership of a file or directory.
- Examples:
  - ```sudo chwon newUser fileName``` changes the ownership of "fileName" to "newUser"
  - ```sudo chown :groupName fileName``` changes the group ownership of "fileName" to "groupName" (remember to user the ```:``` colon)

---

### ```sudo useradd```
- Adds a user to the system.
- Examples:
  - ```sudo useradd -g security newUser``` adds "newUser" as a new user and assigns their primary group to be "security".
  - ```sudo useradd -G finance,admin newUser``` adds "newUser" as a new user and adds them to the existing "finance" and "admin" supplemental groups.

---

### ```sudo usermod```
- Adds a user to the system.
- Examples:
  - ```sudo usermod -g security newUser``` changes newUser's primary group to be "security".
  - ```sudo usermod -G finance,admin newUser``` replaces any existing supplemental groups with the "finance" and "admin" groups.
  - ```soud usermod -a -G finance,admin newUser``` adds "finance" and "admin" groups with the other existing supplemental groups.
  - can use ```-l ``` option to change the user's login name.
  - can use ```-d ``` option to change the user's home directory.
  - can use ```-L ``` option to lock user from logging in. 

---

### ```sudo userdel```
- Removes a user from the system.
- Examples:
  - ```sudo userdel userName``` deletes the user but it doesn't delete the files in the user’s home directory
  - ```sudo userdel -r userName``` deletes the user and all the files in the user’s home directory

---

### ```sudo groupdel```
- Removes a group from the system.

---

### ```sudo groupadd```
- adds a group to the system.

---

### ```man```
- shows how to use a specific command.
- Example: ```man hier```

---

### ```whoami```
- returns the username of the current user
