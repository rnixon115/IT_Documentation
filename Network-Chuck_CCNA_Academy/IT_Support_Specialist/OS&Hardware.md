## Hardware & Types 
1. Punch Cards
2. Paper Tapes
3. Magnetic Tapes
4. Audio Tapes
5. Floppy Disc
6. Flash Drives
7. HDD (Hard Disk Drives) 
8. SSD (Solid State Drives)
9. HHD (Helium Hard Drives)
10. eMMC (Embedded MultiMedia Card)
11. CPU (Central Processing Unit)
12. TPU (Tensor Processing Unit by Google)
13. GPU (Graphics Processing Unit)
14. NPU (Neural Processing Unit for AI)
15. APU ( A CPU combined with a GPU)
16. LPU (Language Processing Unit for LLMs)
17. DPU (Data Processing Unit for Offloading infrastructure)
18. QPU (Quantum Processing Unit, the next frontier)
19. RAM (Random Access Memory)
20. ROM (Read-Only Memory)
21. NIC (Network Interface Card)
22. WNIC (Wireless Network Interface Card)
23. Bluetooth Module
24. Power Supply
25. Motherboard Types [Common: E-ATX (Extended ATX), ATX (Advanced Technology eXtended), Micro-ATX (mATX); Enterprise: Mini-STX (Mini Socket Technology Extended), SSI EEB / SSI CEB (Server System Infrastructure); Companies' Proprietary Form Factors (OEM)]
26. Audio Card
27. Touch Screen
28. RAID Controller (Redundant Array of Independent Disks Controller)
29. CD-ROM (Compact Disc - Read-Only Memory)
30. CD-RW (Compact Disc - Read/Write)


## Windows 
1. Microsoft bought DOS (Disk Operating System), which was then called MS-DOS.
2. Windows 10 and newer are not considered a disk operating system. Instead, Windows 10 is run on NT (New Technology). A fancy term for the OS that's in direct control of the hardware.
3. So, Windows is no longer running a single process but a multitude of processes.
4. Windows computers use multiple types of hardware.

### Windows Hierarchy 
<img width="970" height="683" alt="image" src="https://github.com/user-attachments/assets/147762e9-16f1-4956-addb-a51c137cd3b8" />
Source: Cisco Network Academy, Operating System Basics

### Windows Tools Overview

1. Task Manager
   - Task Manager can show applications running, services, who's signed in, startup apps, CPU usage, Memory usage, Wi-Fi or Ethernet usage, Disk usage, etc. Gives an overview of what's running on the computer.
   - [Task Manager for Windows 11](https://learn.microsoft.com/en-us/shows/inside/task-manager)
2. Event Viewer
   - Keeps a record of everything that happens on the computer. If the computer restarted randomly without explaining why, first look at Event Viewer to see what could've caused the issue.
   - [Event Viewer for Windows 11](https://learn.microsoft.com/en-us/shows/inside/event-viewer)
3. System Information
   - System Information provides an overview of the hardware, operating system version, and other applications in use. If you need to upgrade the RAM or replace another component, check here first to see the specs.
   - [System Information for Windows 11](https://support.microsoft.com/en-us/windows/experience/description-of-microsoft-system-information-msinfo32-exe-tool)  
4. Windows PowerShell (.ps1)
   - Windows PowerShell is a scripting language based on .net. Windows PowerShell uses an object-based {verb}-{noun} naming convention. Windows PowerShell isn't case-sensitive compared to bash or zsh.
   - [What is Windows PowerShell](https://learn.microsoft.com/en-us/powershell/scripting/what-is-windows-powershell?view=powershell-7.6)
     {
        Get-Process
        Get-Childitem
        Get-Printer
        Get-Help
        Get-StorageFileServer
        Get-StartApps
        Get-PnpDevice
        Start-Process
        Set-Variable
        Remove-Printer
        Remove-PrinterDriver
        Remove-NetSwitchTeam
        Remove-NetNeighbor
        Remove-NetIPAddress
     }
5. Command Prompt (CMD)
   - [What Is CMD?](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/cmd)
   {
      dir
      cd {directory}
      cd .. "Moves back one directory
      cd\ "Moves the directory back to root"
      copy {~path\source}
      del {filename}
      find {text in a filename}
      mkdir {directory name}
      ren {rename an old file}
      help "Displays more useful commands and their uses"
   }

## macOS Tools Overview

