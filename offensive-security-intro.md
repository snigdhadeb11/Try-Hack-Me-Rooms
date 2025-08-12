# 🛡️ TryHackMe Write-up — Offensive Security

**Date Completed:** 2025-08-12  
**Difficulty:** Easy  
**Category:** Cybersecurity Fundamentals / Web Exploitation  
**Room Link:** [Offensive Security](https://tryhackme.com/room/offensivesecurity)

---

## 📜 Room Overview
*"To outsmart a hacker, you need to think like one."*

This room introduces the concept of **Offensive Security** — breaking into computer systems, exploiting software bugs, and finding loopholes to gain unauthorized access. The main goal is to understand hacker tactics so we can strengthen system defenses.

You get hands-on practice by hacking a simulated banking application (*FakeBank*) in a safe, legal environment.

---

## 🧠 Key Learnings
- Offensive security involves simulating hacker behavior to find system vulnerabilities.
- Virtual machines can create safe hacking environments for practice.
- Tools like **dirb** can find hidden pages or functionality in websites.
- Brute-forcing URLs is an effective way to discover unintended access points.

---

## 📝 Tasks & Answers

### **Task 1 — What is Offensive Security?**
**Q:** Which of the following options better represents the process where you simulate a hacker's actions to find vulnerabilities in a system?  
**A:** `Offensive Security`

---

### **Task 2 — FakeBank Account Number**
**Q:** What is your bank account number in the FakeBank web application?  
**A:** `8881`

---

### **Task 3 — Your First Hack**
We used the `dirb` tool to brute-force the FakeBank site and discovered two hidden URLs:  
- `http://fakebank.thm/images`  
- `http://fakebank.thm/bank-deposit`

**Q:** What is the other hidden URL (apart from `/images`)?  
**A:** `http://fakebank.thm/bank-deposit`

---

### **Task 4 — Adding Funds**
Visiting `/bank-deposit` allowed us to add `$2000` to our account **8881**. After depositing, a pop-up with green text confirmed success.

**Q:** What are the green words (all in uppercase)?  
**A:** `BANK-HACKED`

---

## 🖼️ Screenshots
*(Optional: Add proof images here)*  
Example:  
`![FakeBank Interface](assets/offensive-security-fakebank.png)`

---

## 🔗 References
- [dirb Documentation](https://tools.kali.org/web-applications/dirb)
- [TryHackMe — Offensive Security](https://tryhackme.com/room/offensivesecurity)

---

## 🏷️ Tags
#offensive-security #web-exploitation #dirb #beginner #easy
