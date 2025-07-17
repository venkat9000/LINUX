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

| Directory | Description | Examples |
|----------|-------------|----------|
| `/` | Root directory: the top-most directory that contains all files and directories | N/A (base of everything) |
| `/bin` | Essential binary executables used by all users | `ls`, `cp`, `mv`, `cat`, `echo`, `pwd`, `touch` |
| `/sbin` | System binaries for system administration, used mostly by root | `reboot`, `shutdown`, `fdisk`, `ifconfig`, `iptables`, `fsck` |
| `/etc` | Configuration files for the system and installed applications | `/etc/passwd`, `/etc/fstab`, `/etc/hostname`, `/etc/ssh/sshd_config` |
| `/home` | Home directories for regular users | `/home/alice`, `/home/bob`, user-specific files like `Documents`, `Downloads` |
| `/dev` | Device files representing hardware | `/dev/sda`, `/dev/null`, `/dev/tty`, `/dev/usb/lp0`, `/dev/random` |
| `/root` | Home directory of the root (superuser/admin) | `/root/.bashrc`, `/root/scripts` |
| `/opt` | Optional third-party or proprietary software packages | `/opt/google/chrome`, `/opt/VirtualBox`, `/opt/myapp` |
| `/lib` | Shared libraries needed by programs in `/bin` and `/sbin` | `/lib/libc.so.6`, `/lib/modules`, `/lib/systemd` |
| `/proc` | Virtual filesystem that provides runtime system info | `/proc/cpuinfo`, `/proc/meminfo`, `/proc/uptime`, `/proc/1/cmdline` |
| `/tmp` | Temporary files used by system and applications, often cleared on reboot | `/tmp/session.lock`, `/tmp/tmp1234.txt` |
| `/usr` | Secondary hierarchy for read-only user data; contains utilities and applications | `/usr/bin`, `/usr/lib`, `/usr/share`, `/usr/local` |
| `/var` | Variable data such as logs, mail, spool files | `/var/log/syslog`, `/var/www`, `/var/spool`, `/var/cache` |
| `/boot` | Files required for booting the system | `/boot/vmlinuz`, `/boot/grub/grub.cfg`, `/boot/initrd.img` |
| `/mnt` | Mount point for temporarily mounting filesystems | `/mnt/usb`, `/mnt/backup` |
| `/media` | Mount point for removable media (USB drives, CDs) | `/media/user/USB_DRIVE`, `/media/cdrom` |
| `/srv` | Data for services provided by the system (e.g., web, FTP) | `/srv/www`, `/srv/ftp` |
| `/run` | Temporary runtime data used by system processes | `/run/systemd`, `/run/user/1000` |



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


