                           
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
