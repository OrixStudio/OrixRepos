# ⚡ tsu-next

> **Next-Generation Su Wrapper for Termux**  
> *Seamless, blazing fast, and universal root execution layer.*

## 🌟 Overview

`tsu-next` is a modern, lightweight, and refined root wrapper designed for **Termux** environments powered by **Magisk**, **KernelSU**, or **APatch**.

It is **NOT** the legacy `tsu` package, but a completely rebuilt next-generation wrapper designed to eliminate permission issues, accelerate root environment startup, and accurately bridge critical environment paths (`PATH`, `HOME`, `LD_LIBRARY_PATH`) with zero latency.

It natively maps to both `tsu` and `tsu-next` binaries, ensuring full backward compatibility with all your scripts and workflows.


## ✨ Key Features

* **⚡ Instant Execution:** Zero-overhead shell spawn for sub-second root access.
* **🔄 Auto-Shell Detection:** Automatically detects and launches your preferred active shell (`zsh`, `bash`, `sh`).
* **🔗 Dual Binary Mapping:** Supports both `tsu` and `tsu-next` syntax natively.
* **🔒 Permission Hardened:** Pre-configured with proper Debian system executable attributes.
* **🛠️ Universal Root Support:** Fully compatible with Magisk, KernelSU, APatch, and standard `su` implementations.

## ⚠️ Prerequisite Step

If you currently have the original `tsu` package installed, **uninstall it first** to avoid binary conflicts:
```bash
pkg remove tsu -y
```

## 🚀 Installation Guide

### Step 1: Add OrixRepos Repository

To access `tsu-next` and other official packages, you must first register the **OrixRepos** repository in your Termux environment.

👉 <a href="https://orixstudio.github.io/OrixRepos" target="_blank"><strong>[CLICK HERE TO OPEN ORIXREPO]</strong></a>

> **Note:** Visit the link above to view the live package tree and copy the repository setup script directly into Termux.

### Step 2: Install Package

Once the repository is added, run the following command to install `tsu-next`:
```bash
pkg update && pkg install tsu-next
```

## 💻 Usage & Commands

You can trigger the root shell using either binary alias:

# Launch root shell using primary alias
```bash
tsu
```

# Launch root shell using next-gen alias
```bash
tsu-next
```

# Display current version
```bash
tsu -v
```

# Display help menu
```bash
tsu -h
```

## 📜 License

Distributed under the MIT License. Developed and maintained by **OrixStudio**.
