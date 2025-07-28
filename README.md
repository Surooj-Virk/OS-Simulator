#  Operating System Simulator (OS Simulator)

An educational simulation of Operating System-level task management and process execution, developed in **C** with optional **GTK-based GUI**. This project mimics a multitasking environment where system resources are allocated, deallocated, and monitored while running various system-like utilities.

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Implemented Tasks](#implemented-tasks)
- [Resource Allocation](#resource-allocation)
- [Kernel Mode](#kernel-mode)
- [Multitasking](#multitasking)
- [GUI Mode](#gui-mode)
- [How to Run](#how-to-run)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [Contributors](#contributors)
- [License](#license)


## About the Project

This project is designed to simulate basic functionalities of an Operating System in a controlled environment using:
- **Terminal-based interface** for minimal interaction.
- **GTK GUI-based interface** for an enhanced user experience.
  
The simulator demonstrates how system utilities, memory, and multitasking operations are handled in a typical OS, including:
- File management
- Task scheduling
- Resource handling
- User interaction



## Features

- Real-time clock and stopwatch
- File creation, renaming, copying, moving, and deleting
- Resource allocation and monitoring
- Calculator and alarm
- Mini Tic-Tac-Toe game
- Contact management system
- Image viewer
- GUI-based and terminal-based notepad, text editor

---

## Implemented Tasks

### Core Tasks (Terminal & GUI)

1. **Timer** - Count down from a user-specified time.
2. **Stop Watch** - Start/stop/reset stopwatch.
3. **Contact Manager** - Add, edit, search, and list contacts.
4. **File Renaming Tool** - Rename existing files.
5. **File Search Tool** - Search for specific words or characters in files.

### Additional Tasks

6. **Mini Game: Tic-Tac-Toe** - Simple 2-player game.
7. **Alarm** - Set alarm using time input.

### Extended Functionalities

8. **Notepad** – Create and save text files (GUI saves on close).
9. **Calculator** – Perform basic arithmetic.
10. **Create File** – Input and save file from terminal.
11. **Move File** – Relocate file to different directory.
12. **Copy File** – Clone a file to a new location.
13. **Delete File** – Remove files from system.
14. **Check File Info** – Display metadata of a file.
15. **Image Viewer** – Load and view an image using GUI.
16. **Text Editor** – Replace contents of a file.


## Resource Allocation

The simulator allocates system resources (RAM, CPU cores, and memory) dynamically. Each task:
- Requests resources upon execution.
- Is denied execution if resources are insufficient.
- Frees resources once completed.

Resources are passed via command-line arguments:

```bash
./os_simulator <RAM_in_MB> <Number_of_Cores> <Memory_in_MB>
