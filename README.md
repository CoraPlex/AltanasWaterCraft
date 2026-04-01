# AWC – AltanasWaterCraft

<p align="center">
  <img src="branding/AWC_final.png" width="500"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-active-brightgreen"/>
  <img src="https://img.shields.io/badge/platform-Windows-blue"/>
  <img src="https://img.shields.io/badge/base-LandSandBoat-orange"/>
</p>

---

Custom Final Fantasy XI Server Base
Built on LandSandBoat – controlled, modified, and maintained by CoraPlex & Vec7rex.

---

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

* Version: 2022 or newer
* ⚠️ REQUIRED: **Desktop development with C++**

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

## 📥 Download AWC

Open a **PowerShell / CMD** window:

```bash
git clone --recursive https://github.com/CoraPlex/AltanasWaterCraft.git
cd AltanasWaterCraft
```

---

## 📦 Install Python Dependencies

```bash
py -3 -m pip install -r server/tools/requirements.txt
```

---

## ⚙️ Setup Configuration

```cmd
xcopy server\settings\default\* server\settings /E /I
```

---

## 🗄 Database Setup

```bash
cd server/tools
py -3 dbtool.py
```

Follow the instructions to create the database (`xidb`)

---

## 🛠 Build Server

* Open **server folder** in Visual Studio
* Wait for:

```text
CMake generation finished
```

Set:

```text
x64-Debug
```

Then:

```text
Build → Build All
```

---

## ✅ Done

```text
Build All succeeded
```

---

## 🚀 Why AWC?

* Simplified setup process
* Clean structure
* Stable base for custom servers
* No unnecessary complexity
* Ready for launcher integration

---

## 📊 Status

Active development

---

## 🙏 Credits

Built on LandSandBoat
https://github.com/LandSandBoat/server

Maintained by:
CoraPlex & Vec7rex

---

## 🛠 Troubleshooting

### Python not recognized

Reinstall Python and enable PATH

---

### dbtool fails

Make sure Python dependencies are installed

---

### Build errors

Check Visual Studio C++ workload and CMake

---
