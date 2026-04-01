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

## 🪟 Windows Installation Guide (AWC)

### 🔹 Requirements

#### Git for Windows

[![Download Git](https://img.shields.io/badge/Download-Git-blue?style=for-the-badge\&logo=git)](https://git-scm.com/download/win)

* Install latest version
* Accept default settings

---

#### Visual Studio

[![Download Visual Studio](https://img.shields.io/badge/Download-Visual%20Studio-purple?style=for-the-badge\&logo=visualstudio)](https://visualstudio.microsoft.com/)

* Version: 2022 or newer
* ⚠️ REQUIRED: **Desktop development with C++**

---

#### MariaDB Server

[![Download MariaDB](https://img.shields.io/badge/Download-MariaDB-orange?style=for-the-badge\&logo=mariadb)](https://mariadb.org/download/)

* Use version **10.6.x**
* Set a root password
* Enable UTF8

⚠️ IMPORTANT:
Enable **UTF8 character set** during installation

---

#### Python 3.12

[![Download Python](https://img.shields.io/badge/Download-Python-yellow?style=for-the-badge\&logo=python)](https://www.python.org/downloads/release/python-3120/)

* Required version: **3.12**
* ✔ Add Python to PATH

---

## 📁 Create Server Folder

Create a new folder (no spaces in the name):

```text id="a1"}
C:\SERVERNAME
```

Right-click → **Open in Terminal**

---

## 📥 Download AWC

```bash id="a2"}
git clone --recursive https://github.com/CoraPlex/AltanasWaterCraft.git
cd AltanasWaterCraft
```

Wait until the process finishes.

---

## ⚙️ Configure Settings

Copy all `.lua` files from:

```text id="a3"}
server\settings\default
```

to:

```text id="a4"}
server\settings
```

---

Open:

```text id="a5"}
server\settings\Network.lua
```

Edit:

```lua id="a6"}
SQL_PASSWORD = 'YOUR_PASSWORD'
```

---

## 🗄 Database Setup

```bash id="a7"}
cd server/tools
py -3 dbtool.py
```

Enter MariaDB path:

```text id="a8"}
C:\Program Files\MariaDB 10.6\bin
```

Confirm database creation:

```text id="a9"}
y
```

Then exit:

```text id="a10"}
q
```

---

## 🛠 Build Server

* Open **Visual Studio**
* Select: **Open Folder**
* Choose:

```text id="a11"}
C:\SERVERNAME\AltanasWaterCraft\server
```

Wait until:

```text id="a12"}
CMake generation finished
```

---

## ▶️ Build

Set:

```text id="a13"}
x64-Debug
```

Then:

```text id="a14"}
Build → Build All
```

---

## ✅ Done

```text id="a15"}
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

Ensure Python dependencies are installed

---

### Build errors

Check Visual Studio C++ workload and CMake

---
