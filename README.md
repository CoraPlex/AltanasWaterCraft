# AWC – AltanasWaterCraft

<p align="center">
  <img src="branding/AWC_final.png" width="700"/>
</p>

---

**AWC is a streamlined Final Fantasy XI server base built on LandSandBoat.
Designed for simplicity, stability, and easy setup.**

---

## 📌 Navigation

* [🪟 Windows Installation Guide](#-windows-installation-guide-awc)
* [🚀 Why AWC?](#-why-awc)
* [📊 Status](#-status)
* [🙏 Credits](#-credits)
* [🛠 Troubleshooting](#-troubleshooting)

---

## 🪟 Windows Installation Guide (AWC)

### 🔹 Requirements

#### Git

https://git-scm.com/download/win

#### Visual Studio

https://visualstudio.microsoft.com/

⚠️ REQUIRED:
**Desktop development with C++**

---

#### MariaDB

https://mariadb.org/download/

* Use version 10.6.x
* Set root password
* Enable UTF8

---

#### Python 3.12

https://www.python.org/downloads/release/python-3120/

✔ Add to PATH

---

## 📥 Installation

Open CMD or PowerShell:

```bash
git clone --recursive https://github.com/CoraPlex/AltanasWaterCraft.git
cd AltanasWaterCraft
```

---

## 📦 Install Dependencies

```bash
py -3 -m pip install -r tools/requirements.txt
```

---

## ⚙️ Setup Configuration

```cmd
xcopy settings\default\* settings /E /I
```

---

## 🗄 Database Setup

```bash
py -3 tools/dbtool.py
```

---

## 🛠 Build Server

* Open project folder in Visual Studio
* Wait for: **CMake generation finished**

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

Reinstall Python and enable PATH option

---

### dbtool fails

Make sure dependencies are installed

---

### Build errors

Check Visual Studio C++ workload and CMake

---
