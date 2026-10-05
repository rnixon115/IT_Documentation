
## Windows Updates, Feature Updates, Driver Updates, and Optional Updates

1. Quality Updates (Patch Tuesday Updates) – Released monthly with security and reliability fixes.
2. Feature Updates – Major updates introducing new functionality (e.g., Windows 10 to Windows 11 upgrades).
3. Driver and Firmware Updates – Updates for hardware components, sometimes included in Windows Update.
4. Optional Updates – Feature enhancements and non-security updates that require manual installation.

#### Users & Groups

- Administrator: An admin is a user with full control of the computer and folders. Note: Unless the operating system is Windows 
- Users: Users can perform common tasks on a workstation by running applications, accessing a local printer, etc.
- Guest: A guest is a temporary profile that is created and deleted from signing in to the computer to signing off.
  
#### Linux & macOS

- Linux and macOS have similar roles. Linux has Owner, Groups, and Others. Each one 

#### Permissions 
| Permission | Description |
| :--------: | :---------: |
| Full Control | Allows for complete access to the computer, files, folders, modifying permissions, and taking ownership. |
| Modify | Allows reading, writing, and deleting files and folders, but not changing permissions. |
| Read & Execute | Allows the user to read a file and execute applications. |
| List Folder Contents | Displays files, folders, and subdirectories. |
| Read | Allows a user to get the content of a file or folder. | 
| Write | Allows a user to create new files and edit existing ones. |

#### Steps to Reset a Password in Local Users and Groups Manager
1. Log in as an Admin.
2. Open Users and Groups Manager.
3. Go to the "Users" folder.
4. Right-click on the user's name and select "Set Password".
5. Click on "Proceed" in the warning box.
6. Type a new password and confirm.

#### Steps to Reset a Password in Active Directory  

1. Open up the Run box and type in "dsa.msc".
2. Find the user's account by searching for the user folder and search by the username of the user.
3. Right-click the user's name and select Password 

## macOS & Linux Ubuntu Distro

- Linux & macOS are descendants of Unix, which was created in 1969 at Bell Labs.
- Linux was developed by Linus Torvalds, who wanted a free alternative to Unix that anyone can modify.

##### macOS & Ubuntu Tips:
  1. Keychain is a security credential manager embedded in macOS.
  2. Gnome-Keying is a security credential manager embedded in Ubuntu.
  3. Signautre contains sample code used by viruses/malware.
  5. Firmware is the lowest-level functionality for a device.
  6. Patches update minor or major common vulnerabilities from third-party companies.
  7. Cron is a service that can schedule a process to run a script, application, or command.

##### Virtualization
  1. Virtualization allows the user to run a virtualized computer inside a machine.
- ###### There are two types of virtualization: Type-1 Hypervisor & Type-2 Hypervisor
  - A Type-1 Hypervisor runs on bare metal or hardware. This allows for multiple instances to run on a machine without passing through the main OS's.
  - <img width="356" height="192" alt="image" src="https://github.com/user-attachments/assets/9c60a096-a5af-458c-b637-56b8af094362" />
  - A Type-2 Hypervisor sits on top of the OS's and acts as a guest. The guest can use resources, but only the host dictates which resources it can use.
  - <img width="298" height="209" alt="image" src="https://github.com/user-attachments/assets/46da3c73-3cdd-4edd-8b4c-3f9659eeef08" />




