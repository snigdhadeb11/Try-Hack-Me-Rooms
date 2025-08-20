# Windows Fundamentals 2 Walkthrough

This repository contains a structured walkthrough for the TryHackMe room "Windows Fundamentals 2." It is designed to provide a comprehensive guide, including theoretical concepts, practical steps, and all the correct answers to the room's questions.

This module continues the journey of exploring the Windows operating system, focusing on various utilities and management tools that are essential for system administration and troubleshooting.

## Table of Contents
- [Task 1: Introduction](#task-1-introduction)
- [Task 2: System Configuration](#task-2-system-configuration)
- [Task 3: Change UAC Settings](#task-3-change-uac-settings)
- [Task 4: Computer Management](#task-4-computer-management)
- [Task 5: System Information](#task-5-system-information)
- [Task 6: Resource Monitor](#task-6-resource-monitor)
- [Task 7: Command Prompt](#task-7-command-prompt)
- [Task 8: Registry Editor](#task-8-registry-editor)
- [Task 9: Conclusion](#task-9-conclusion)

---

## Task 1: Introduction

This task provides an overview of the room's content and prompts the user to start the virtual machine.

No questions to answer in this task.

---

## Task 2: System Configuration

**Theory:**
The **System Configuration (MSConfig)** utility is a powerful tool for diagnosing Windows startup issues. It's a key part of an administrator's toolkit for troubleshooting. The utility is organized into five tabs:
- **General:** Allows you to select the type of startup (Normal, Diagnostic, or Selective).
- **Boot:** Provides advanced boot options for the operating system.
- **Services:** Lists all system services, whether running or stopped.
- **Startup:** Redirects you to the Task Manager to manage startup applications.
- **Tools:** Provides a list of other useful Windows utilities that can be launched directly from here.

**Question:** What is the name of the service that lists Systems Internals as the manufacturer?
- **Answer:** `Sysmon`

**Question:** Whom is the Windows license registered to?
- **Answer:** `Administrator`

**Question:** What is the command for Windows Troubleshooting?
- **Answer:** `C:\Windows\System32\msdt.exe -id PCWDiagnostic`

**Question:** What command will open the Control Panel? (The answer is the name of .exe, not the full path)
- **Answer:** `control.exe`

---

## Task 3: Change UAC Settings

**Theory:**
**User Account Control (UAC)** is a security feature that prompts users for permission before allowing actions that require elevated privileges. The UAC settings can be configured to be more or less restrictive, though it is not recommended to turn them off completely. The settings are controlled via a slider that modifies how and when UAC prompts appear.

**Question:** What is the command to open User Account Control Settings? (The answer is the name of the .exe file, not the full path)
- **Answer:** `UserAccountControlSettings.exe`

---

## Task 4: Computer Management

**Theory:**
The **Computer Management (compmgmt.msc)** utility is a comprehensive console that consolidates several administrative tools into one interface. It is organized into three main sections:
- **System Tools:** Includes **Task Scheduler**, **Event Viewer** (for viewing system logs), **Shared Folders**, **Local Users and Groups**, **Performance Monitor**, and **Device Manager**.
- **Storage:** Contains **Disk Management** for managing disk partitions and volumes.
- **Services and Applications:** Lists all system services and provides access to the **Windows Management Instrumentation (WMI)** control.

**Question:** What is the command to open Computer Management? (The answer is the name of the .msc file, not the full path)
- **Answer:** `compmgmt.msc`

**Question:** At what time every day is the GoogleUpdateTaskMachineUA task configured to run?
- **Answer:** `8:05 AM`

**Question:** What is the name of the hidden folder that is shared?
- **Answer:** `C$`

---

## Task 5: System Information

**Theory:**
The **System Information (msinfo32.exe)** tool provides a detailed overview of the computer's hardware, system components, and software environment. This information is crucial for diagnosing issues and understanding the system's specifications. The tool is divided into three sections:
- **Hardware Resources:** Technical details about hardware.
- **Components:** Specific information about devices like displays and input devices.
- **Software Environment:** Details about the operating system and installed applications, including **Environment Variables**.

**Question:** What is the command to open System Information? (The answer is the name of the .exe file, not the full path)
- **Answer:** `msinfo32.exe`

**Question:** What is listed under System Name?
- **Answer:** `THM-JOHN`

**Question:** Under Environment Variables, what is the value for ComSpec?
- **Answer:** `%SystemRoot%\system32\cmd.exe`

---

## Task 6: Resource Monitor

**Theory:**
**Resource Monitor (resmon.exe)** is an advanced monitoring tool that provides real-time data on the usage of system resources. It is particularly useful for troubleshooting performance bottlenecks. It offers detailed views for:
- **CPU:** Process activity and CPU usage.
- **Disk:** Disk I/O activity.
- **Network:** Network traffic and connections.
- **Memory:** Memory usage by process.

**Question:** What is the command to open Resource Monitor? (The answer is the name of the .exe file, not the full path)
- **Answer:** `resmon.exe`

---

## Task 7: Command Prompt

**Theory:**
The **Command Prompt (cmd.exe)** is a command-line interpreter that allows users to interact with the Windows operating system by typing commands. While GUIs have become the primary method of interaction, the command prompt remains essential for automation, scripting, and advanced tasks. Key commands for system information and troubleshooting include:
- `hostname`: Displays the computer's name.
- `whoami`: Shows the current logged-in user.
- `ipconfig`: Displays network configuration settings.
- `netstat`: Shows network connections and statistics.
- `net`: Used to manage network resources and users.

**Question:** In System Configuration, what is the full command for Internet Protocol Configuration?
- **Answer:** `C:\Windows\System32\ipconfig.exe`

**Question:** For the ipconfig command, how do you show detailed information?
- **Answer:** `ipconfig /all`

---

## Task 8: Registry Editor

**Theory:**
The **Windows Registry** is a hierarchical database that stores configuration settings and options for the operating system and applications. It is a critical component of Windows, and making incorrect changes can cause system instability. The **Registry Editor (regedit.exe)** is the tool used to view and modify the registry. This tool should only be used by advanced users.

**Question:** What is the command to open the Registry Editor? (The answer is the name of the .exe file, not the full path)
- **Answer:** `regedit.exe`

---

## Task 9: Conclusion

This task concludes the room and summarizes the utilities covered, emphasizing that they can be launched from multiple locations, not just MSConfig.

No questions to answer in this task.
