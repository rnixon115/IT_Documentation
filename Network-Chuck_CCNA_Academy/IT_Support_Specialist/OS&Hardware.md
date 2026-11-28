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

## Serial Connectivity

#### Legacy Ports

   1. Serial ports were once used to connect peripherals like printers and modems. Today, they are still occasionally used for console connections to configure network devices. The two main types of serial ports are the 9-pin DB-9 and the 25-pin port.nd the 25-pin port.
   2. Parallel ports have a 25-pin connector for connecting peripheral devices. They transmit multiple bits of data simultaneously, which is why they are commonly known as printer ports, as they were often used for printers.
   3. The 15-pin game port was used for joystick input, initially on dedicated game controller cards and later integrated into sound cards and PC motherboards.
   4. The PS/2 is a 6-pin DIN connector for connecting a keyboard and mouse, with purple for the keyboard and green for the mouse.
   5. Audio ports connect devices to computers, including a line-in for external sources, a microphone port, and line-out ports for speakers or headphones.

#### Video Ports & Connectors

1. The Video Graphics Array (VGA) is an old analog port still found on some PCs but is becoming obsolete. It is blue in color and uses a 15-pin connector arranged in three rows.
2. The Digital Visual Interface (DVI) was created with the rise of digital displays like LCD monitors and TVs for transmitting uncompressed digital video. DVI has several variants: 
- **DVI-A** (Analog) for analog signals only  
- **DVI-D** (Digital) for digital signals only  
- **DVI-I** (Integrated) for both  
There are also two types of connections: single-link, using one TMDS transmitter, and dual-link, using two TMDS transmitters for higher resolutions. The standard DVI connector is white and can have up to 24 pins for digital signals, 4 pins for analog signals, and a ground bar.
3. High-Definition Multimedia Interface (HDMI) was designed for high-definition televisions but is also suitable for computers. It transmits video, audio, and control signals through a 19-pin connector. A smaller version, Mini-HDMI, is available for portable devices. HDMI supports high resolutions and can adjust the monitor's refresh rate to match the source output. The most common connectors are Type A (Standard), Type C (Mini), and Type D (Micro).
4. DisplayPort is a modern technology meant to replace DVI and VGA for connecting monitors, using a 20-pin connector for high-bandwidth video and audio. There’s also a Mini DisplayPort version, mainly for Apple computers. It connects high-end PCs and displays, supporting up to 80 Gbps with versions 2.0 and 2.1. Additionally, DisplayPort can connect multiple monitors to one video source using a single cable.
5. The USB Type-C connector is a compact, rectangular interface with rounded corners, designed to connect various peripheral devices to a PC. It serves as both USB and Thunderbolt 3, offering functionality for data transfer, video output, and power delivery through a single cable.

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
       1. Get-Process
       2. Get-ChildItem
       3. Get-Printer
       4. Get-Help
       5. Get-StorageFileServer
       6. Get-StartApps
       7. Get-PnpDevice
       8. Start-Process
       9. Set-Variable
       10. Remove-Printer
       11. Remove-PrinterDriver
       12. Remove-NetSwitchTeam
       13. Remove-NetNeighbor
       14. Remove-NetIPAddress
     
5. Command Prompt (CMD)
   - [What Is CMD?](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/cmd)
   1. dir
   2. cd {directory}
   3. cd .. "Moves back one directory
   4. cd\ "Moves the directory back to root"
   5. copy {~path\source}
   6. del {filename}
   7. find {text in a filename}
   8. mkdir {directory name}
   9. ren {rename an old file}
   10. help "Displays more useful commands and their uses"
   

## macOS Tools Overview

- About This Mac is an important overview of the system and what the Mac is running on. About This Mac lists the processor (CPU), memory(RAM), Serial Number, and Operating System Version. [macOS Activity Monitor](https://support.apple.com/guide/activity-monitor/welcome/mac)
- System Settings is the control panel for macOS. You can adjust the display, user accounts, security settings, network configuration, and more. [System Settings for Tahoe 26](https://support.apple.com/guide/activity-monitor/welcome/mac)
- Mac has a built-in log viewer called Console. Console gives users the capability to see what happened. Why an app crashed, why the system shut down, what services aren't running, etc. [What is Console](https://support.apple.com/guide/console/welcome/mac)


  
