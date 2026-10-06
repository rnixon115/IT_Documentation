
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
   - <img width="570" height="337" alt="image" src="https://github.com/user-attachments/assets/b5a4db4f-9c39-4ce5-85ef-9dee1f3e8d4e" />
3. Go to the "Users" folder.
   - <img width="1467" height="816" alt="image" src="https://github.com/user-attachments/assets/16d543b1-66b9-4c14-aef1-fdcfe3f3078e" />
5. Right-click on the user's name and select "Set Password".
   - <img width="1467" height="816" alt="image" src="https://github.com/user-attachments/assets/41782067-c286-464f-8d42-50d4be6f009b" />
7. Click on "Proceed" in the warning box.
   - <img width="1467" height="816" alt="image" src="https://github.com/user-attachments/assets/685b172c-4e5a-475e-a4f9-f80590bc0d81" />
9. Type a new password and confirm.
   - <img width="1467" height="816" alt="image" src="https://github.com/user-attachments/assets/e58fb25b-2dda-481e-9a37-898c9a7c1130" />

#### Steps to Reset a Password in Active Directory  

1. Open up the Run box and type in "dsa.msc".
   - <img width="572" height="339" alt="image" src="https://github.com/user-attachments/assets/fafde53d-7183-4deb-88f8-43743f59349d" />
2. Find the user's account by searching for the user folder and searching by the user's username.
   - <img width="751" height="526" alt="image" src="https://github.com/user-attachments/assets/a988039d-a142-4cd6-9240-cc7caa185d75" />
3. Right-click the user's name and select Password.
   - <img width="750" height="528" alt="image" src="https://github.com/user-attachments/assets/a0cc48e7-116d-49ba-a410-c3f25e98dff0" />
4. Enter the password and confirm it.
   - <img width="748" height="527" alt="image" src="https://github.com/user-attachments/assets/b90c9c7a-42d6-43cc-8aa0-7fce76d98826" />
5. Select "ok"
   - <img width="378" height="257" alt="image" src="https://github.com/user-attachments/assets/69ccce23-7bb1-4d77-97c2-fe284d6721d2" />

#### Steps to Unlock AD Account Lockouts

1. Open Active Directory & Users and Computers.
   - <img width="1176" height="888" alt="image" src="https://github.com/user-attachments/assets/cca8e8f1-5d18-4194-bf92-28849e76cb46" />
2. Locate the account and select the account properties.
   - <img width="1175" height="784" alt="image" src="https://github.com/user-attachments/assets/6b83424a-c0bb-48ef-b52a-ae67301feefd" />
3. Unlock the Account
   - <img width="1174" height="790" alt="image" src="https://github.com/user-attachments/assets/629ceda2-324c-4346-946a-d15a7ee50617" />

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




