# rfalturism-linux
# UMU-Proton + Faugus GUI Guide for RF Online (Altruism)

This guide shows how to download, register, and run **RF Online (Altruism)** on Linux using **UMU-Proton-9.0-4e** and **Faugus GUI**, with a proper **32-bit prefix**.

---

## 📑 Table of Contents
- [Step 1: Download the Game](#-step-1-download-the-game)
- [Step 2: Register with Altruism](#-step-2-register-with-altruism)
- [Step 3: Create a Game Account](#-step-3-create-a-game-account)
- [Create a 32-bit UMU-Proton Prefix](#-create-a-32-bit-umu-proton-prefix)
- [Install Dependencies with Winetricks](#-install-dependencies-with-winetricks)
- [Launch the Game](#-launch-the-game)
- [Remove a Prefix](#-remove-a-prefix)
- [Manual Prefix Management (Advanced)](#-manual-prefix-management-advanced)
- [License](#-license)

---

## 🎮 Step 1: Download the Game

👉 [**Download the game here**](https://rfaltruism.com/download)  

Start the download, and while waiting, move on to the next steps.

⚠️ **Important:**  
Your antivirus or browser may block some files.  
These are **false positives** — the files are safe.  

✅ No harmful software is installed.  
✅ No information is collected from your PC.  

Once the download finishes and is installed, you can log in using your game account (see Step 3) via **RF Altruism Launcher**.

---

## 📝 Step 2: Register with Altruism

👉 [**Register your account here**](https://rfaltruism.com/register)  

A community account is required to manage game accounts and access all website features.

---

## 🕹️ Step 3: Create a Game Account

1. Log in to the [**Altruism Dashboard**](https://rfaltruism.com/dashboard).  
2. Go to **Game Accounts**.  
3. Create your first game account.  

ℹ️ **Tip:**  
- RF Online has many races, classes, and cross-classes.  
- Most players eventually need multiple accounts, but start with one to log in via **RF Altruism Launcher**.

---

## 🔧 Create a 32-bit UMU-Proton Prefix

1. Open a terminal.  
2. Run the following commands to create a clean **32-bit prefix**:

```bash
# Create a 32-bit prefix
WINEPREFIX=/home/yourname/wineprefixes/umu-rfalturism32 WINEARCH=win32 \
~/.local/share/Steam/compatibilitytools.d/UMU-Proton-9.0-4e/files/bin/wineboot

⚙️ Install Dependencies with Winetricks
Install the required components:

bash
￼Kopiera kod
WINEPREFIX=/home/yourname/wineprefixes/umu-rfalturism32 winetricks \
w_workaround_wine_bug-50894 vcrun2015 d3dx9 winxp dotnet48 gdiplus
w_workaround_wine_bug-50894 → fixes a known Wine bug.

vcrun2015 → Visual C++ 2015 runtime.

d3dx9 → DirectX 9.

winxp → sets Windows version to XP.

dotnet48 → .NET Framework 4.8.

gdiplus → required graphics library for launchers.

🚀 Launch the Game
Open Faugus GUI.

Select your umu-rfalturism32 prefix.

Click Run executable in prefix.

Select RF_Altruism_Launcher.exe from the game folder.

Log in with your game account.

📂 Manual Prefix Management (Advanced)
All UMU-Proton prefixes are stored here:

swift
￼Kopiera kod
~/.local/share/Steam/compatibilitytools.d/UMU-Proton-9.0-4e/files/share/default_pfx/
To manage your custom 32-bit prefix:

bash
￼Kopiera kod
WINEPREFIX=/home/yourname/wineprefixes/umu-rfalturism32 winecfg
📜 License
Free to use and share.

￼


