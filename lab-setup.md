# LAB SETUP

The lab environment consisted of three virtual machines configured to simulate an enterprise Active Directory network.

## Virtual Machines

**• Domain Controller: Windows Server 2019**\
**• Client Machine: Windows 10**\
**• Attacker Machine: Kali Linux**

<figure><img src=".gitbook/assets/Screenshot 2026-03-21 111412.png" alt=""><figcaption></figcaption></figure>

## **Network Configuration**

The environment was configured using a Host-Only network to simulate an internal enterprise environment. All systems were placed within the same subnet to enable communication between attacker and target machines.

Example IP assignments:\
• Domain Controller: 192.168.56.50\
• Kali Linux: 192.168.56.102\
• Domain Name: Abhi.local
