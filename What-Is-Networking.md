# What is Networking?  

---

## Course Overview

Networking is the concept of connecting devices so they can communicate and share data. Networks are everywhere — from friendships to city infrastructure — and in computing, networking connects technological devices like phones, laptops, and even traffic lights. Understanding networking is essential for cybersecurity and modern technology.

---

## Task 1: What is Networking?

**What is Networking?**

Networks are simply things connected. For example, your friendship circle: you are all connected because of similar interests, hobbies, skills, and so on.

Networks can be found in all walks of life:  
- A city's public transportation system  
- Infrastructure such as the national power grid for electricity  
- Meeting and greeting your neighbours  
- Postal systems for sending letters and parcels  

In computing, networking is the same idea but dispersed to technological devices. Take your phone as an example; the reason you have it is to access things. Devices communicate with each other by following rules.

A network can be formed by anywhere from 2 devices to billions, including laptops, phones, security cameras, traffic lights, farming equipment, and more.

Networks are integrated into everyday life — gathering weather data, delivering electricity, and controlling traffic flow.

**Key Term:**  
Devices connected together form a **Network**.

---

## Task 2: What is the Internet?

The Internet is one giant network made up of many smaller networks connected together.

Imagine Alice has new friends Zayn and Toby she wants to introduce to Bob and Jim, but only Alice speaks their language. Alice acts as a messenger connecting these smaller groups, forming a larger network.

### History of the Internet:
- Originated from the ARPANET project in the late 1960s, funded by the US Defence Department.  
- The Internet as we know it was created by **Tim Berners-Lee** in 1989 with the invention of the World Wide Web (WWW).  

### Types of Networks:
- **Private Network:** A smaller network of connected devices.  
- **Public Network:** Networks connecting private networks together; this is the Internet.

**Answer:**  
Who invented the World Wide Web?  
**Tim Berners-Lee**

---

## Task 3: Identifying Devices on a Network

Devices must identify themselves to communicate properly.

### Two ways of identification (like humans):

| Human Analogy | Device Equivalent          |
|---------------|---------------------------|
| Name          | IP Address                |
| Fingerprints  | MAC Address               |

### IP Address (Internet Protocol)

- Identifies a device on a network for a certain time.  
- Consists of 4 sections called **octets** (e.g., 192.168.1.77).  
- IP Addresses change from device to device but can't be duplicated on the same network simultaneously.  
- Two types:  
  - **Private IP Address:** Identifies device within a private network.  
  - **Public IP Address:** Identifies device on the Internet, assigned by ISP.  

#### IPv4 vs IPv6:
- IPv4: Uses 32-bit addressing (about 4.29 billion addresses).  
- IPv6: Uses 128-bit addressing (about 340 trillion addresses), solves IPv4 shortage.

### MAC Address (Media Access Control)

- Physical address assigned to network interface hardware (NIC).  
- Format: 12 hexadecimal digits separated by colons, e.g., `a4:c3:f0:85:ac:2d`.  
- First 6 digits: Manufacturer ID.  
- Last 6 digits: Unique device number.  
- MAC addresses can be **spoofed**, potentially breaking some security assumptions.

### Key Terms & Answers:

| Question                                   | Answer                 |
|--------------------------------------------|------------------------|
| What does "IP" stand for?                   | Internet Protocol      |
| What is each section of an IP address called?| Octet                  |
| How many sections (digits) does an IPv4 address have?| 4                    |
| What does "MAC" stand for?                   | Media Access Control   |

### Interactive Lab Flag

```plaintext
THM{YOU_GOT_ON_TRYHACKME}
Task 4: Ping (ICMP)
Ping is a fundamental network tool used to test connectivity between devices.

Uses ICMP (Internet Control Message Protocol) packets.

Sends an "echo request" to the target device and waits for an "echo reply".

Measures the time (latency) packets take to travel.

Usage
Ping can be used to check connection to IP addresses or websites. It's available on most operating systems.

Ping Syntax Example:

bash
Copy code
ping 10.10.10.10
Key Questions & Answers
Question	Answer
What protocol does ping use?	ICMP
What is the syntax to ping 10.10.10.10?	ping 10.10.10.10
What flag do you get when you ping 8.8.8.8?	THM{I_PINGED_THE_SERVER}

<img width="1919" height="853" alt="image" src="https://github.com/user-attachments/assets/00eaac9a-bd51-4230-aa77-70464ef8f019" />
