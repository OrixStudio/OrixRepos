# ⚡ tsu-next

> **Next-Generation Su Wrapper for Termux**  
> *Seamless, blazing fast, and universal root execution layer.*

---

## 🌟 Overview

`tsu-next` is a modern, lightweight, and refined root wrapper designed for **Termux** environments powered by **Magisk**, **KernelSU**, or **APatch**. 

It is **NOT** the legacy `tsu` project, but a completely rebuilt next-generation wrapper designed to fix permission bugs, speed up root environment initialization, and handle environment variables (`PATH`, `HOME`, `LD_LIBRARY_PATH`) natively without overhead.

It binds directly to both `tsu` and `tsu-next` binaries, ensuring 100% backward compatibility with all your scripts.

---

## ✨ Features

- **⚡ Instant Execution:** Zero-bloat initialization for sub-second root shell spawn.
- **🔄 Auto-Shell Detection:** Automatically inherits your active environment shell (`zsh`, `bash`, `sh`).
- **🔗 Dual Binary Mapping:** Works with both `tsu` and `tsu-next` commands.
- **🔒 Native Permission Handling:** Built-in standard Debian file permissions.
- **🛠️ Universal Root Compatibility:** Works flawlessly with Magisk, KernelSU, APatch, and standard `su`.

---

## ⚠️ Important Note Before Installation

If you have the old, legacy `tsu` package installed, **you must uninstall it first** to prevent binary collision:

pkg remove tsu -y

---

## 🚀 Quick Setup & Installation

### Step 1: Add OrixRepos Repository

To install `tsu-next`, you need to add the **OrixRepos** master repository to your Termux package sources.

👉 <a href="[https://orixstudio.github.io/OrixRepos](https://orixstudio.github.io/OrixRepos)" target="_blank">**Click Here to Visit OrixRepos for Live Package Tree & Commands**</a>

Or run this single command to add the repository directly:

echo "deb [trusted=yes] [https://orixstudio.github.io/OrixRepos](https://orixstudio.github.io/OrixRepos) ./" > $PREFIX/etc/apt/sources.list.d/orix.list

### Step 2: Install tsu-next

Update your package index and install the tool:

pkg update && pkg install tsu-next

---

## 💻 Usage

Simply invoke either `tsu` or `tsu-next` from your Termux prompt:

# Launch root shell
tsu

# Alternative command
tsu-next

# Check installed version
tsu -v

# View help menu
tsu -h

---

## 📜 License

Distributed under the MIT License. Developed and maintained by **OrixStudio**.
