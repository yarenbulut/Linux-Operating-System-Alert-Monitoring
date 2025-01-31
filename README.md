# **Linux Operating System Alert Monitoring**

## **Stress Testing and Monitoring with Telegram Bot on VirtualBox and Ubuntu**

---

## 📌 **Project Description**
This project aims to:
- Create a virtual machine using VirtualBox
- Install the Ubuntu Server operating system
- Format disks and perform stress testing
- Monitor system resources
- Send alerts through a Telegram bot

---

## 📖 **Table of Contents**
1. **Installation**
   - Download and install VirtualBox
   - Create a new virtual machine
   - Install Ubuntu Server
2. **Ubuntu Server Installation**
   - Virtual machine setup
   - Memory and disk configuration
   - Ubuntu installation
3. **Filesystem Creation**
   - Adding and formatting a second disk
   - Creating a mount point
   - Configuring automatic mounting
4. **Stress Testing**
   - Writing a Bash script for stress testing
   - Running the script
5. **Creating a Telegram Bot**
   - Setting up a bot using BotFather
   - Writing a Python script for monitoring
6. **Resource Monitoring and Alerts**
   - Installing required Python libraries
   - Writing a monitoring script
7. **Results and Discussion**
8. **Conclusion**

---

## ⚙️ **Installation**

### **1️⃣ Download and Install VirtualBox**
- Download the latest version of VirtualBox from the [official website](https://www.virtualbox.org/wiki/Downloads)
- Install it on your system

### **2️⃣ Create a New Virtual Machine**
- Open VirtualBox and create a new virtual machine
- Configure memory and disk sizes as needed

### **3️⃣ Install Ubuntu Server**
- Download Ubuntu Server from the [official Ubuntu website](https://ubuntu.com/download/server)
- Install it on your virtual machine

---

## 📥 **Ubuntu Server Installation**

### **1️⃣ Create a Virtual Machine**
- Open VirtualBox and create a virtual machine for Ubuntu Server

### **2️⃣ Configure Memory and Disk Sizes**
- Adjust memory and disk sizes according to system requirements

### **3️⃣ Install and Configure Ubuntu**
- Follow the standard installation process for Ubuntu Server

---

## 📂 **Filesystem Creation**

### **1️⃣ Add a Second Disk and Format It as XFS**

```bash
mkfs.xfs /dev/sdb
```

### **2️⃣ Create a Mount Point**

```bash
mkdir /khas
```

### **3️⃣ Mount the Disk and Configure Automatic Mounting**

Edit the `/etc/fstab` file to ensure the disk mounts automatically at startup:

```bash
/dev/sdb /khas xfs defaults 0 0
```

---

## 🏋️ **Stress Testing**

### **1️⃣ Create a Bash Script for Stress Testing**
- Create a script named `stressTest.sh` that includes commands for testing CPU, memory, and disk usage

### **2️⃣ Run the Script**
- Execute the script to simulate high system load

---

## 🤖 **Creating a Telegram Bot**

### **1️⃣ Set Up a Telegram Bot Using BotFather**
- Use **BotFather** on Telegram to create a new bot
- Obtain your **API token** for authentication

### **2️⃣ Write a Python Script for System Monitoring and Alerts**
- Develop a Python script to monitor system load and send alerts via Telegram

---

## 📊 **Resource Monitoring and Alerts**

### **1️⃣ Install Required Python Libraries**

```bash
pip install psutil python-telegram-bot
```

### **2️⃣ Write and Run the Monitoring Script**
- Develop a Python script to track system resource usage
- Send alerts to Telegram when predefined thresholds are exceeded

---

## 📈 **Results and Discussion**
This project successfully:
- Created a virtual machine with Ubuntu Server
- Formatted and managed disk partitions
- Conducted system stress testing
- Implemented Telegram-based monitoring and alerting

The findings help analyze system performance in a virtualized environment and highlight potential issues in real-world usage scenarios.

---

## 🏁 **Conclusion**
This project provides a complete solution for:
✅ **Virtual machine setup**
✅ **Filesystem management**
✅ **Stress testing**
✅ **Resource monitoring** via Telegram bot

It serves as a useful tool for **system administrators and developers** who need efficient monitoring in virtualized environments.


