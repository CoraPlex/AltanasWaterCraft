# AWC – AltanasWaterCraft

<p align="center">
  <img src="branding/AWC_final.png" width="700"/>
</p>

---

Custom Final Fantasy XI Server Base  
Built on LandSandBoat – controlled, modified, and maintained by CoraPlex & Vec7rex.


## 🪟 Windows Installation Guide

### Install Requirements

#### 🔹 Git for Windows

[![Download Git](https://img.shields.io/badge/Download-Git-blue?style=for-the-badge\&logo=git)](https://git-scm.com/download/win)

* Latest version is fine
* Accept defaults
* Change default text editor if desired

---

#### 🔹 Visual Studio

[![Download Visual Studio](https://img.shields.io/badge/Download-Visual%20Studio-purple?style=for-the-badge\&logo=visualstudio)](https://visualstudio.microsoft.com/)

* 2022 or newer
* ⚠️ You MUST install:
  **Desktop development with C++**

---

#### 🔹 MariaDB Server

[![Download MariaDB](https://img.shields.io/badge/Download-MariaDB-orange?style=for-the-badge\&logo=mariadb)](https://mariadb.org/download/)

* Use version **10.6.x**
* Set root password
* Use UTF8

⚠️ IMPORTANT:
Enable **UTF8 character set** during installation

---

#### 🔹 Python 3.12

[![Download Python](https://img.shields.io/badge/Download-Python-yellow?style=for-the-badge\&logo=python)](https://www.python.org/downloads/release/python-3120/)

* Required version: **3.12**
* ✔ Add python.exe to PATH

---

### Download AWC & Setup

Open a **PowerShell/CMD** window and navigate to your chosen install directory.

```bash
git clone --recursive https://github.com/CoraPlex/AltanasWaterCraft.git
```

---

Install Python requirements:

```bash
py -3 -m pip install -r server/tools/requirements.txt
```
Close **PowerShell/CMD**

---

### Setup Database

Open a **PowerShell/CMD** window in your tools folder.

```bash
py -3 dbtool.py
```

Follow instructions to create database (`xidb`)

---

### Build Server

* Open **server folder** in Visual Studio
* Wait for:

```text
CMake generation finished
```

Set:

```text
x64-Debug
```

Build:

```text
Build → Build All
```

---

### ✅ Done

```text
Build All succeeded
```
