                           
# **Linux-commands** 

## How to Open the Terminal?

  • Shortcut keys: Ctrl+Alt+T (Ubuntu-based distros).
    
   • Search "Terminal" in the application menu.
    
  • Use a virtual console: Ctrl+Alt+F1 to F6 (return to GUI with Ctrl+Alt+F7).                    

## Basics of Command Syntax
  
### Structure of a Command:

      command [options] [arguments]
      
  • Command: The program you want to run (e.g., ls to list files).
  
  • Options: Modify the behavior of the command (e.g., -l for long format).
  
  • Arguments: The file, directory, or data you want the command to work on.


### Examples:

    • ls -l /home → List files in long format in /home.
    
    • cp file.txt /tmp → Copy file.txt to /tmp.

## File and Directory Operations

1. Navigating Directories:
   
        ◦ pwd → Print current directory path.
     
        ◦ cd [path] → Change directory.
     
            ▪ cd /home → Go to /home.
            ▪ cd .. → Move up one level.

   
2. Listing Files:
   
        ◦ ls → List files in the current directory.
   
        ◦ ls -a → Include hidden files.
   
        ◦ ls -l → Display details like permissions and size.

   
  3. Creating and Removing:
     
          ◦ touch filename → Create an empty file.
       
          ◦ mkdir dirname → Create a directory.
       
          ◦ rm filename → Remove a file.
       
          ◦ rm -r dirname → Remove a directory recursively.
     
  4. Moving and Copying Files:
   
          ◦ mv file1 file2 → Rename file1 to file2.
       
          ◦ mv file /path/ → Move file to /path/.
       
          ◦ cp file /path/ → Copy file to /path/.


# Viewing and Editing Files

  1. Display File Contents:
     
          ◦ cat file → Display the content of a file.
       
          ◦ less file → View file one screen at a time.
       
          ◦ head -n 10 file → Display the first 10 lines of a file.
       
          ◦ tail -n 10 file → Display the last 10 lines.

     
  2. Editing Files:
     
          ◦ nano file → Open a simple text editor.
       
          ◦ vim file → Open a powerful editor (requires learning commands like i to insert, :wq to save and exit).


# Managing Processes

  1. Check Running Processes:
     
          ◦ ps → Show active processes.
       
          ◦ top or htop → Interactive process monitoring.
  
          
  2. Kill Processes:
     
          ◦ kill PID → Kill a process by its ID.
       
          ◦ killall name → Kill processes by name.


# Permissions and Ownership

  1. View File Permissions:
     
          ◦ ls -l → Shows permissions as drwxr-xr-x.
          
              ▪ d → Directory.
              
              ▪ r → Read, w → Write, x → Execute.

            
  3. Change Permissions:
    
          ◦ chmod → Modify file permissions.
          
              ▪ Example: chmod 755 file → Owner can read/write/execute, others can read/execute.
            
  4. Change Ownership:
    
          ◦ chown user:group file → Change file owner and group.


# Network Commands

  1. Check Network Configuration:
    
          ◦ ifconfig or ip addr → Show network interfaces.
          ◦ ping [hostname] → Test connectivity.

        
  2. Download Files:
    
          ◦ wget URL → Download files from a URL.


# Package Management

  1. Installing/Removing Software (Debian-based distros like Ubuntu):
    
          ◦ sudo apt update → Update package list.
          
          ◦ sudo apt install package → Install a package.
          
          ◦ sudo apt remove package → Remove a package.

        
  2. For RedHat-based Distros:
    
          ◦ yum or dnf → Use similar commands.


# Shell Scripting Basics

  1. Create a Script:
     
  ◦ Create a file with .sh extension:
          
          #!/bin/bash
          echo "Hello, Linux!"
          
  ◦ Make it executable: chmod +x script.sh.
  
  ◦ Run the script: ./script.sh.
  

  2. Loops and Conditions:
       
         for i in {1..5}; do
             echo "Count $i"
         done



# Advanced Tips
  1. Searching Files:
     
          ◦ grep "text" file → Search for text in a file.
       
          ◦ find /path -name "filename" → Locate files.

     
  2. Archiving and Compressing:
     
          ◦ tar -czvf archive.tar.gz /path → Compress files into a tarball.

     
  3. Permissions for Multiple Files:

          ◦ chmod -R 755 /path → Change permissions recursively.
