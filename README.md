# Linux Permissions

This project explains the fundamentals of the Linux file permission system, provides a visual flowchart, and how to set file permissions.

  
## File Permissions

File permissions control who can read, write, or execute a file. When you use `ls -l` command, you see a 10-character string like `-rwxr-xr--`.

| **File Type** | **Owner** | **Group** | **Others** |
| :---: | :---: | :---: | :---: |
| `-`   | `rwx` | `r-x` | `r--` |

1.  **File Type:** The first character. `-` means it's a regular file, and `d` means it's a directory.
2.  **Owner Permissions:** The next three characters (`rwx`). These are the permissions for the user who owns the file.
3.  **Group Permissions:** The next three characters (`r-x`). These are the permissions for members of the group the file belongs to.
4.  **Others Permissions:** The final three characters (`r--`). These are the permissions for all other users on the system.

## Permissions Meanings

Each group of three characters defines the rights for that user class:
* `r` **Read** permission.
* `w` **Write** permission.
* `x` **Execute** permission.
* `-` **No permission** is granted.

## Permissions Flowchart

<img width="600" height="800" alt="image" src="https://github.com/user-attachments/assets/2a57b413-b500-42bd-af77-0108d2ce9cce"/>

## Applying `rwxrwxr-x` Permissions

The goal is to set a file's permissions to `rwxrwxr-x`.
These permission translates to "Read-Write-Execute" to the owner of the file and "Read-Write-Execute" to the group of the owner and "Read-Execute" to other users.

<img width="1000" height="800" alt="brave_1972" src="https://github.com/user-attachments/assets/4ec998f9-1b3f-4f45-b6ec-acf9e3396bad"/>
