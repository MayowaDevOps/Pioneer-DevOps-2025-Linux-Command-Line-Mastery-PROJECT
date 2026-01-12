# Pioneer-DevOps-2025-Linux-Command-Line-Mastery-PROJECT

---

# 1. Linux File System Navigation


# DevOps.linux.navigation
Overview
This section demonstrates practical understanding of Linux file system navigation, file inspection, and directory management using core command line tools on an Ubuntu system. The tasks were executed using standard Linux utilities to explore system directories, locate files, and inspect file attributes.

Activities Performed
1.1 Current Working Directory
The pwd command was used to display the absolute path of the current working directory, confirming awareness of location within the file system.
---
### ![pwd](./img/img-pwd1.PNG)

## 1.2 Listing Files in the Home Directory
The ls -la command was executed in the home directory to display all files, including hidden files, along with permissions, ownership, and file sizes.

### ![ls-la](./img/img-lsla2.PNG)



## 1.3 Navigating to System Directories

The cd /etc command was used to change into the system configuration directory, and ls was used to list its contents.

### ![cd](./img/img-cd3.PNG)

## 1.4 Relative Path Navigation

From the /etc directory, relative paths were used to navigate back to the home directory, demonstrating understanding of directory hierarchy and relative navigation.
### ![homedir](./img/img-homedir4.PNG)

## 1.5 Directory Toggle

The cd - command was used to toggle between the current and previous directories, confirming familiarity with quick navigation shortcuts.
### ![togglecurrent](./img/img-togglecurrent5.PNG)

## 1.6 Locating the Bash Binary

### ![whereisbash](./img/img-whereisbash6.PNG)
The whereis bash command was used to display the absolute path of the bash executable on the system.

## 1.7 File Search Across the System
### ![psswd](./img/img-psswd7.PNG)

The find / -type f -name "passwd" command was executed to locate files named passwd across the filesystem, verifying file search capability.

## 1.8 Directory Tree Visualization
The tree utility was installed and used to display the directory structure of the user’s home directory (/home/mayowa-ubuntu) in a tree format.
### ![installtree](./img/img-installtree8.PNG)

## 1.9 Disk Usage Summary
### ![dush](./img/img-dush9.PNG)

The du -sh * command was used to summarize disk usage of files and directories in the current working directory.

## 1.10 File Type Identification

The file /etc/hosts command was used to identify the file type of the hosts file.

### ![countdir](./img/img-countdir11.PNG)

## 1.11 Counting Directories

### ![countdir](./img/img-countdir11.PNG)
A combination of ls -l, grep, and wc was used to count the number of directories in the /etc directory.


## 1.12 Symbolic Link Verification

The ls -l /bin/sh command was used to verify the symbolic link path and confirm what /bin/sh points to on the system.

### ![symbactivity](./img/img-verifysymbactivity12.PNG)

---
Conclusion
This section confirms hands-on proficiency in Linux file system navigation, directory inspection, file searching, and command usage. The commands executed align with the requirements of the Linux and Command Line Mastery mini project and demonstrate readiness for further DevOps foundational tasks.


## 2. Linux Program Management

# Overview

This section demonstrates the ability to install, verify, and manage software packages and services on Ubuntu Linux. It covers installing utilities, validating program availability, and installing and managing the Nginx web server using system service controls.
Activities Performed


## 2.1 Updating Package Repositories
The sudo apt update command was used to refresh package lists and ensure the system had the latest repository metadata.
### ![pwd](img./img-pwd01.PNG)


## 2.2 Installing Required Programs
The sudo apt install command was used to install tree, nano, and nginx, demonstrating package installation skills.
## ![pwd](img./img-pwd2.PNG)

## 2.3 Verifying Installations
Installed tools were validated using version checks such as tree --version and nginx -v, confirming successful installation.
## ![pwd](img./img-pwd3.PNG)

## 2.4 Confirming Executable Paths
The which and whereis commands were used to confirm binary locations and verify program availability in the system environment.
## ![pwd](img./img-pwd4.PNG)

## 2.5 Editing Files with Nano
The nano editor was used to create or edit a test file, demonstrating basic command-line text editing and saving.

## ![pwd](img./img-pwd5.PNG)

## 2.6 Inspecting Nginx Configuration Structure
The tree /etc/nginx command was used to inspect the structure of Nginx configuration directories and files.
## ![pwd](img./img-pwd6.PNG)

## 2.7 Starting and Enabling Nginx
The sudo systemctl start nginx command was used to start Nginx, and sudo systemctl enable nginx was used to enable auto-start on boot.
## ![pwd](img./img-pwd7.PNG)

## 2.8 Checking Nginx Status
The sudo systemctl status nginx command was used to confirm the web server service is running properly.
## ![pwd](img./img-pwd8.PNG)

## 2.9 Verifying Port 80 Listening
The ss -tuln | grep 80 command was used to confirm Nginx was actively listening on port 80.

## ![pwd](img./img-pwd9.PNG)
## 2.10 Removing and Reinstalling a Package
A package was removed using sudo apt remove and reinstalled using sudo apt install, confirming software lifecycle management.

## 2.11 Searching for Packages
The apt-cache search nano command was used to locate package names in repositories, demonstrating package discovery.

## ![pwd](img./img-pwd10.PNG)
## Conclusion

This section confirms hands-on proficiency in software installation, verification, and service management on Ubuntu. It also demonstrates practical ability to manage a web server service using systemctl.



# 3. Linux File Management

## Overview

This section demonstrates practical skills in creating, modifying, copying, moving, and deleting files and directories in Linux. It also includes file inspection and metadata checks used in day-to-day DevOps operations.
## Activities Performed

## 3.1 - 3.5 Creating Directories
The mkdir and mkdir -p commands were used to create directories and nested directory structures.



## 3.2 Creating Files
Files were created using touch, confirming basic file creation capability.

## 3.3 Writing and Appending Content
Text was written and appended into files using redirection operators (> and >>), demonstrating overwrite and append behavior.

## 3.4 Viewing File Contents
The cat command was used to display file contents and confirm correct edits.

## 3.5 Copying Files
The cp command was used to copy files into another directory, demonstrating file duplication and organization.

## ![pwd](img../img-pwd1234.PNG)

## 3.6 - 3.9  Moving and Renaming Files
The mv command was used to rename files and move them where necessary.
## ![mkdirc](./img../img-mkdirc6789.PNG)

## 3.7 Deleting Files and Directories
The rm command was used for file deletion, and rmdir was used to remove empty directories safely.


## 3.8 Previewing File Content
The head and tail commands were used to preview file content from the start and end.


## 3.9 Checking File Metadata
The stat command was used to inspect file metadata including timestamps, permissions, and ownership.


## 3.10 Counting Lines in a File

The wc -l command was used to count the number of lines in a file.

## ![rmempty.di](img../img-rmempty.di10.PNG)

## 3.11 Creating Multiple Files Efficiently
Brace expansion was used to create multiple files at once (e.g., file{1..5}.log).

## ![headandtailmkdir](img../img-headandtailmkdir11.PNG)

## ![metadata](img../img-metadata12.PNG)

## ![countnumbers](img../img-countnumbers13.PNG)

## ![display](img../img-display%20hrf1415.PNG)
## 3.12 Human-Readable File Listing
The ls -lh command was used to display file sizes in a readable format.


#  Conclusion
This section confirms the ability to manage files and directories effectively, inspect file details, and perform routine file operations required in DevOps workflows.


## 4. Linux File Permissions and Ownership

## Overview

This section demonstrates understanding and practical application of Linux permissions, ownership, and advanced directory permission settings. Tasks included modifying file permissions, changing ownership/group, using umask, and applying special permission bits (sticky bit and SGID).

## Activities Performed

## 4.1 Viewing Permissions and Ownership

The ls -l command was used to view file permissions, ownership, and group assignments.

## ![currentpermission](img.../img-currentpermission1.PNG)

## 4.2 - 4.4 Changing Permissions Using chmod
Permissions were updated using numeric modes (e.g., chmod 644, chmod 755) and symbolic modes (e.g., chmod u+x, chmod g-w).


## 4.3 Changing File Ownership and Group
The chown command was used to change file ownership, and chgrp was used to change group ownership.


## 4.4 Applying Recursive Permissions
The chmod -R command was used to apply permissions across directories and their contents.

## ![chgpermission](img.../img-chgpermissionrmg234.PNG)

## 4.5 Verifying Permission Changes
The stat command was used to validate updated permissions and ownership settings.


## 4.6 Testing Default Permissions with umask
The umask value was checked and updated, then tested by creating a new file and confirming its default permissions.

## ![changeownergroup](img.../img-changeownergroup56.PNG)
## 4.7 Configuring a Sticky Bit Directory
A shared directory was configured using chmod 1777, and ls -ld was used to confirm the sticky bit (t) is applied.

## ![permission](img.../img-permissioncopy7.PNG)

## 4.8 Configuring an SGID Directory
A directory was configured using chmod 2775 to ensure new files inherit the directory’s group ownership.

##![verifystat](img.../img-verifystat8.PNG)

## 4.9 Comparing Symbolic vs Numeric Permissions
Permissions were adjusted using both numeric and symbolic formats to demonstrate flexibility and understanding.

## ![default](img.../img-defaultpermission9.PNG)

## ![share](img.../img-sharedstickybit1011.PNG)

## ![sgid](img.../img-SGID12.PNG)

## ![sudo](img.../img-sudochangeownerhip1314.PNG)

## ![explore](img.../img-explorepermission15.PNG)

## Conclusion
This section confirms practical capability in Linux access control, ownership management, and secure directory configuration, which are essential for multi-user system administration and DevOps operations.


## 5. Linux Redirection and Command Chaining

## Overview

This section demonstrates the ability to redirect outputs, capture errors, chain commands, and process data using pipelines. These techniques are essential for scripting, automation, troubleshooting, and log analysis in DevOps environments.

## Activities Performed


## 5.1 - 5.3 Redirecting Output to Files

Standard output was redirected using > to write results to a file, and >> was used to append outputs to an existing file.


## 5.2 Redirecting Errors to Files
Standard error was redirected using 2> to capture error messages into an error log file.

## ![standarderror](img..../img-rstandarderror3.PNG)
## 5.3 Redirecting Both Output and Errors
The &> operator was used to capture both standard output and standard error into a single file.


## 5.4 Filtering Output with grep
The grep command was used to search for specific keywords within files and outputs.

## ![combin](img..../img-combinestdout4.PNG)
## 5.5 -5.6  Using Pipelines for Processing
Pipelines (|) were used to chain commands like cat, grep, and wc for filtering and counting results.


## 5.6 Sorting and Removing Duplicates
Text output was processed using sort and uniq to organize and remove duplicates.

## ![filter](img..../img-filtercontexample56.PNG)

## 5.7 Extracting Fields from /etc/passwd
The cut and awk commands were used to extract specific fields from /etc/passwd, demonstrating structured parsing.

## ![sortuniq](img..../img-sortuniq7.PNG)

## 5.8 Text Replacement Using sed
The sed command was used to replace text within a file, demonstrating automated content editing.


## 5.9 Command Chaining with && and ||
Commands were chained with && to run subsequent commands only if the previous succeeded, and || to handle failure cases.

## ![awk](img..../img-awk89.PNG)

## 5.10 Timing a Command

The time command was used to measure how long a command takes to execute.

## ![replace](img..../img-replace10.PNG)

## ![occurence](img..../img-occurence11.PNG)

## ![redirect](img..../img-redirect&append12.PNG)

## ![pipelines](img..../img-pipelines013.PNG)

## ## ![testoutput](img..../img-testoutput14.PNG)

## Conclusion

This section confirms strong understanding of Linux I/O redirection, pipelines, and command chaining. These skills support automation and efficient troubleshooting in production environments.



6. Linux Process Management

## Overview

This section demonstrates the ability to inspect and monitor running processes, manage services, and review system resource usage. It also includes interactive monitoring using htop, which is useful for live troubleshooting.


## Activities Performed

## 6.1 Viewing Running Processes
The ps aux command was used to list active processes and view CPU/memory usage.

## ![listprocess](img...../img-listprocess1.PNG)

## 6.2 Monitoring Processes in Real Time
The top command was used to monitor processes interactively and observe resource consumption in real time.

## ![topcpu2](img...../img-topCPU2.PNG)

## 6.3 Locating Nginx Process IDs
The pidof nginx command (or filtering via ps) was used to identify process IDs related to Nginx.

## ![finfnginx](img...../img-findnginxPID3.PNG)

## 6.4 - 6.6 Restarting and Verifying Services
The Nginx service was restarted using systemctl restart nginx and verified using systemctl status nginx.


## 6.5 Checking System Uptime and Load
The uptime command was used to check system uptime and load averages.


## 6.6 Checking Disk Usage
The df -h command was used to review disk usage and available space.

## ![killandrestart](img...../img-killandrestart456.PNG)
## 6.7 Checking Memory Usage
The free -m command was used to view memory usage in megabytes.


## 6.8 Inspecting CPU Information
The lscpu command was used to display CPU details and system architecture information.


## 6.9 Checking Kernel Version
The uname -r command was used to confirm the running kernel version.

## ![directory](img...../img-directory%20size9.PNG)

## 6.10 Listing Running Services
The systemctl list-units --type=service output was used to view currently running services.

## ![memory](img...../img-memorydisplay10.PNG)
## 6.11 Background Process Handling

A command was executed in the background using &, and jobs was used to confirm background job tracking.

## ![cpudetails](img...../img-CPUdetails11.PNG)

## 6.12 Interactive Monitoring Using htop


## ![kenneluptime](img...../img-kennelUPTIME12.PNG)

## ![uningservices](img...../img-unningservices13.PNG)

## ![background](img...../img-background_process1415.PNG)

The htop utility was installed (if not already available) and used to explore interactive monitoring features such as sorting by CPU/memory usage and searching/filtering processes.


## Conclusion

This section confirms hands-on capability in Linux process monitoring, service management, system resource inspection, and interactive troubleshooting using standard Linux tools.
