# Ubuntu 24.04 LTS on Apple Silicon (M1 / M2 / M3) using UTM

Oluwaseyi Michael Falode | Cloud & Cybersecurity | Toronto, ON

A self-directed **CloudOps & Cybersecurity** project demonstrating how to virtualize and configure **Ubuntu 24.04 LTS (ARM Architecture)** on Apple Silicon Macs using **UTM**, a lightweight virtualization tool for macOS.  

> **Goal:** Build foundational Linux and virtualization skills essential for managing and securing cloud environments.

---

## 🎯 Objectives
- Learn how to **virtualize Ubuntu ARM** on Apple Silicon.  
- Configure **UTM** to run Ubuntu 24.04 LTS with a **Graphical User Interface (GUI)**.  
- Install guest tools to improve performance and integration.  
- Practice **Linux command-line administration** for CloudOps & Cybersecurity tasks.  

---

## 🧰 Technologies

| Category | Tools / Versions |
|-----------|------------------|
| **Host OS** | macOS (Apple Silicon M1 / M2 / M3) |
| **Virtualization** | UTM for macOS |
| **Guest OS** | Ubuntu 24.04 LTS (ARM Architecture) |
| **Utilities** | `tasksel`, `APT Package Manager`, `spice-vdagent`, `spice-webdavd` |

---

## ⚙️ Step-by-Step Guide

### 🪄 **Step 1 – Download UTM**
- Visit [UTM Official Site](https://mac.getutm.app/) or [UTM GitHub](https://github.com/utmapp/UTM).  
- Download the latest version, drag it into **Applications**, and launch it.

---

### 💿 **Step 2 – Download Ubuntu ARM Image**
- Go to [Ubuntu ARM Downloads](https://ubuntu.com/download/server/arm).  
- Choose **Ubuntu 24.04 LTS (ARM Server Image)** for Apple Silicon.

---

### 🖥️ **Step 3 – Create a New VM in UTM**
1. Click **“Create a New Virtual Machine” → Virtualize**.  
2. Select **ARM64 Architecture**.  
3. Attach the **Ubuntu ARM ISO** you downloaded.  
4. Allocate CPU & RAM (e.g., 4 CPUs and 4–8 GB RAM).  
5. Complete setup and start the VM.

---

### ⚡ **Step 4 – Install Ubuntu 24.04 LTS**
- Follow the on-screen installation prompts.  
- Set up your **username, password, and preferences**.

---

### 🧩 **Step 5 – Install GUI and Guest Tools (for Better Performance)**

After successfully installing Ubuntu 24.04 LTS, it’s time to set up a **desktop environment (GUI)** and **guest tools** to enhance your virtualization experience.  
These steps make Ubuntu smoother to use — improving graphics, clipboard sharing, file transfer, and window resizing.

#### 🖥️ Install GUI (Ubuntu Desktop Environment)
Run the following commands inside your Ubuntu terminal:

```bash
sudo apt update
sudo apt install tasksel
sudo apt install ubuntu-desktop

### **⚙️ Step 6 – Install Guest Tools (SPICE Integration) (Optional)** 

To further improve performance and system stability, you can install optional utilities or performance monitoring tools.

```bash
sudo apt install htop
sudo apt install neofetch

