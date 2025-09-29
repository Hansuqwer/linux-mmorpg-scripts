---
layout: post
title: "Ragnarok Online (uaRO)"
date: 2025-09-29
---

## About
uaRO is a private Ragnarok Online server.  
This script helps you set it up on Linux.

## Script
```bash
#!/bin/bash
# Ragnarok Online uaRO installer
WINEPREFIX="$HOME/.wine-uaRO"
export WINEPREFIX
wine "$HOME/Games/uaRO_Full_Client/Uaro.exe"
```

## Notes
- Requires Wine and winetricks.
- Tested on Arch Linux with Wine 10.15.
