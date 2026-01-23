# Hytale Mod Manager

A custom PySide6 client for managing Hytale resources via the CurseForge API. This tool automates the organization of mods and worlds.

This manager was built because CurseForge provides no native support for Hytale on Linux.

---

## 🚀 Setup Guide

### 1. Obtaining a CurseForge API Key
CurseForge requires an API Key to fetch mod data.
1.  Go to the [CurseForge for Studios](https://console.curseforge.com/#/) portal.
2.  Log in with your CurseForge/Overwolf account.
3.  Click on **"Create New App"**.
4.  Give your app a name (e.g., `MyHytaleManager`).
5.  Once created, copy the **API Key** from the dashboard.
6.  In the Hytale Mod Manager, click **🔑 Set API Key** in the sidebar and paste your key.



### 2. Finding your Hytale Folder Path
The manager needs to know where Hytale is installed to sort your files correctly.

#### **If using the Hytale Launcher:**
1.  Open the **Hytale Launcher**.
2.  Go to **Settings** (usually a gear icon ⚙️).
3.  Look for **"Open Directory"**.

### 3. Applying the Path
1.  Open the Manager and click **⚙ Game Folder** at the bottom of the sidebar.
2.  Navigate to the path found in the step above.
3.  Ensure you select the **root Hytale folder** (the one containing the `UserData` folder).

---

## 📂 How it Works (Auto-Sorting)
The manager automatically detects the resource type and appends the correct subfolder:
* **Mods:** Sorted into `UserData/Mods`
* **Worlds:** Automatically unzipped into `UserData/Saves`

---

## 🛠 Tech Stack
* **Language:** Python 3
* **UI Framework:** PySide6 (Qt)
* **API:** CurseForge
* **Platform:** Any, focus on Linux