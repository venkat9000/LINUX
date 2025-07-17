# 📘 What is Linux?

**Linux** is an open-source operating system based on **Unix**, widely used for **servers**, **cloud computing**, and **embedded systems**.

## ✅ Key Features:
- **Operating System**: Manages hardware and software resources.
- **Open Source**: Free to use, modify, and distribute.
- **Developed in 1991** by Linus Torvalds.
- **Multi-User & Multi-Tasking**: Many people can use the system simultaneously, and it can run multiple tasks concurrently.
- **Case Sensitive**: Treats uppercase and lowercase differently (`File.txt` ≠ `file.txt`).

---

## 📦 Linux Distributions (Flavors)

A **distribution (distro)** is a customized version of Linux that includes the OS, package management, and additional tools.

| Distro   | Use Case                                      |
|----------|-----------------------------------------------|
| RedHat   | Enterprise-grade, commercial support (RHEL)   |
| Ubuntu   | User-friendly, widely used for desktops/servers |
| CentOS   | Community-supported version of RedHat         |
| Debian   | Stable, known for reliability                 |
| SUSE     | Enterprise use, strong in SAP environments    |
| Others   | Fedora, Arch Linux, Kali Linux (for penetration testing), etc. |

---


## 🗂️ Linux Directory Structure

<img width="580" height="267" alt="image" src="https://github.com/user-attachments/assets/367db036-2c23-41e7-b892-e7114fc6acbc" />


Linux follows a **hierarchical directory structure** starting from `/` (root directory).


### 🔍 Key Directories Explained

| Directory | Description |
|----------|-------------|
| `/`      | Root directory: top-most directory |
| `/bin`   | Essential binary executables (e.g., `ls`, `cp`, `mv`) |
| `/sbin`  | System binaries for administration (e.g., `reboot`, `fdisk`) |
| `/etc`   | Configuration files (e.g., `/etc/passwd`) |
| `/home`  | User directories (`/home/user1`, `/home/user2`) |
| `/dev`   | Hardware devices as files (e.g., `/dev/sda`) |
| `/root`  | Home directory of the root (admin) user |
| `/opt`   | Optional third-party software packages |
| `/lib`   | Shared libraries required by system binaries |
| `/proc`  | Virtual filesystem providing system info (e.g., `/proc/cpuinfo`) |
| `/tmp`   | Temporary files, cleared on reboot |

---

## 📌 Linux Interview Questions (IQ)

### 🔹 1. What is the difference between `/bin` and `/sbin`?

#### 📁 `/bin` (Binary Executables)
- Contains basic commands available to **all users**
- Essential for basic system operations
- **No root privileges** required

**Examples:**
- `ls` – List directory contents
- `cat` – View file contents
- `cp` – Copy files
- `mv` – Move or rename files
- `rm` – Remove files

#### 📁 `/sbin` (System Binaries)
- System administration commands used by **root**
- Used for system maintenance
- **Requires root privileges** (via `sudo`)

**Examples:**
- `shutdown` – Power off the system
- `reboot` – Restart the system
- `ifconfig` – Configure network interfaces
- `mount` – Mount filesystems
- `fsck` – File system consistency check

---

### 🔹 2. In which directory are all external software packages installed?

📁 **Answer: `/opt`**

- Used to store **optional (third-party)** software
- Not part of the default Linux distribution
- Suitable for commercial software, large apps, or manually installed tools

**Examples:**
- Google Chrome → `/opt/google/chrome`
- VirtualBox → `/opt/VirtualBox`
- Custom enterprise apps

**💡 Why `/opt`?**
- Keeps system directories clean
- Prevents conflict with default installations (like `/usr/bin`)
- Simplifies management of third-party apps

---

## 📌 Summary

| Directory | Purpose                         | Access Level      | Examples                         |
|----------|----------------------------------|-------------------|----------------------------------|
| `/bin`   | Essential user commands          | All users         | `ls`, `cp`, `mv`, `rm`           |
| `/sbin`  | System administration commands   | Root user (sudo)  | `shutdown`, `reboot`, `mount`    |
| `/opt`   | External software packages       | Varies by package | Google Chrome, VirtualBox        |

---


