# Introduction to Windows Walkthrough

This repository contains a structured walkthrough for the TryHackMe room "Introduction to Windows." It's designed to help users navigate the room, understand the key concepts, and find the correct answers to the tasks.

The "Introduction to Windows" room provides a general overview of the Windows operating system, covering its user interface, file system, user accounts, and essential utilities like Task Manager.

## Table of Contents
- [Task 1: Introduction to Windows](#task-1-introduction-to-windows)
- [Task 2: Windows Editions](#task-2-windows-editions)
- [Task 3: The Desktop (GUI)](#task-3-the-desktop-gui)
- [Task 4: The File System](#task-4-the-file-system)
- [Task 5: User Accounts, Profiles, and Permissions](#task-5-user-accounts-profiles-and-permissions)
- [Task 6: User Account Control](#task-6-user-account-control)
- [Task 7: Settings and the Control Panel](#task-7-settings-and-the-control-panel)
- [Task 8: Task Manager](#task-8-task-manager)
- [Task 9: Conclusion](#task-9-conclusion)

---

## Task 1: Introduction to Windows

This task introduces the virtual machine and the overall scope of the room.
No questions to answer.

---

## Task 2: Windows Editions

**Theory:**
Windows has a long history, with different versions aimed at specific user needs. The room mentions key versions like Windows XP, Vista, 7, 8.x, 10, and the current Windows 11. It highlights the difference between consumer-focused versions (like Home) and business-focused versions (like Pro) which include additional features for security and management. BitLocker is a full-disk encryption feature that is a prime example of a security tool found in the Pro edition but not the Home edition.

**Question:** What encryption can you enable on Pro that you can't enable in Home?
- **Answer:** `BitLocker`

---

## Task 3: The Desktop (GUI)

**Theory:**
The Windows Desktop is the primary graphical user interface (GUI) and is composed of several key components:
- **Desktop:** The main screen where you can place shortcuts for quick access.
- **Start Menu:** Provides access to all installed applications, files, and system settings. It is broken into sections for your account, all apps, and "tiles."
- **Taskbar:** A bar at the bottom of the screen that displays open applications and provides access to pinned shortcuts.
- **Notification Area:** Located on the right side of the taskbar, it shows the time, date, and icons for system notifications and background applications.

**Question:** Which selection will hide/disable the Search box?
- **Answer:** `Hidden`

**Question:** Which selection will hide/disable the Task View button?
- **Answer:** `Show Task View button`

**Question:** Besides Clock and Network, what other icon is visible in the Notification Area?
- **Answer:** `Action Center`

---

## Task 4: The File System

**Theory:**
The New Technology File System (NTFS) is the standard file system for modern Windows installations. It is a significant improvement over older file systems like FAT due to its enhanced features:
- **Journaling:** It keeps a log of file system changes, allowing for automatic repair in case of a system failure.
- **Permissions:** It allows administrators to set granular permissions (Full control, Modify, Read, etc.) on files and folders, controlling who can access or change them.
- **Compression and Encryption:** Supports on-the-fly compression and encryption of data.
- **Alternate Data Streams (ADS):** A feature that allows files to contain more than one stream of data. This can be used for legitimate purposes but has also been exploited by malware to hide data.

**Question:** What is the meaning of NTFS?
- **Answer:** `New Technology File System`

---

## Task 5: User Accounts, Profiles, and Permissions

**Theory:**
Windows manages users through accounts, which fall into two primary types:
- **Administrator:** Has full control over the system, including the ability to add/remove users, install software, and change system-level settings.
- **Standard User:** Can only make changes to their own files and settings and cannot perform system-level changes without an administrator's permission.
Each user account has a **profile**, which is a folder located at `C:\Users\` that stores the user's personal files and settings (e.g., Desktop, Documents, Downloads). User accounts can also be members of **groups**, inheriting the permissions of that group. The **Local User and Group Management (`lusrmgr.msc`)** tool provides a detailed view of all users and groups on the system.

**Question:** What is the name of the other user account?
- **Answer:** `tryhackmebilly`

**Question:** What groups is this user a member of?
- **Answer:** `Remote Desktop Users,Users`

**Question:** What built-in account is for guest access to the computer?
- **Answer:** `Guest`

**Question:** What is the account description?
- **Answer:** `window$Fun1!`

---

## Task 6: User Account Control

**Theory:**
User Account Control (UAC) is a security feature introduced to mitigate the risks of running with elevated privileges. When an administrative task is initiated, UAC presents a prompt that requires the user's confirmation before the action can proceed. This prevents malicious software from making unauthorized system changes without the user's knowledge. The presence of a shield icon on a program's shortcut indicates that it requires UAC elevation to run.

**Question:** What does UAC mean?
- **Answer:** `User Account Control`

---

## Task 7: Settings and the Control Panel

**Theory:**
Windows provides two main interfaces for system configuration:
- **Control Panel:** The traditional configuration tool that has been a part of Windows for many years. It provides access to a wide range of advanced and complex settings, often organized by categories.
- **Settings:** A more modern, touch-friendly interface introduced in Windows 8. It's designed for simplicity and ease of use, providing access to common settings in a streamlined manner. While some settings are unique to one or the other, many tasks can be performed in both, and sometimes, a task started in **Settings** will redirect you to the **Control Panel** for more detailed options.

**Question:** In the Control Panel, change the view to Small icons. What is the last setting in the Control Panel view?
- **Answer:** `Windows Defender Firewall`

---

## Task 8: Task Manager

**Theory:**
Task Manager is a vital utility for system monitoring and management. It provides real-time information about:
- **Processes:** All running applications, background processes, and services, along with their resource consumption (CPU, Memory, Disk, Network).
- **Performance:** Graphs and data on the overall usage of hardware components like the CPU, RAM, and Disk.
- **Startup:** A list of applications that automatically start when the computer boots.
- **Users:** Information on logged-in users and their resource usage.
It can be accessed quickly by right-clicking the taskbar or using the `Ctrl+Shift+Esc` keyboard shortcut.

**Question:** What is the keyboard shortcut to open Task Manager?
- **Answer:** `Ctrl+Shift+Esc`

---

## Task 9: Conclusion

This is the final task, which wraps up the room and prompts the user to terminate the virtual machine.
No questions to answer.
