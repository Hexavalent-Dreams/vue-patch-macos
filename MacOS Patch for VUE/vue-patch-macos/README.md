
# VUE Resurrection Patch for macOS (Java 6 Launcher Fix)

**Author:** Dez + GPT Tech Priestess 🖤  
**Purpose:** This project provides a workaround to launch the legacy app **VUE (Visual Understanding Environment)** on modern macOS systems where Java 6 support has been dropped and SIP/Gatekeeper protections block normal execution.

## 🎯 What This Patch Does
- Installs Java 6 manually (extracted from Apple's `.pkg`)
- Bypasses System Integrity Protection where necessary
- Hijacks VUE's launcher with a shell script to manually inject `JAVA_HOME` and `DYLD_LIBRARY_PATH`
- (Planned) Rebuilds the `.app` with native launcher wrapper for broader compatibility

## 🧰 Requirements
- macOS (tested on Big Sur–Monterey)
- Terminal access
- Ability to disable SIP (temporarily)
- Java 6 DMG from Apple: https://support.apple.com/kb/DL1572
- VUE.app from Tufts University (no longer maintained)

## 🧱 File Structure (Planned)
```
vue-patch-macos/
├── README.md
├── vue_launcher_patch.sh
├── java6_manual_install.sh
├── screenshots/
└── docs/
    └── VUE_Resurrection_Protocol_Dez_MacOS.txt
```

## ✅ Steps (Simplified)
1. Disable SIP temporarily via Recovery Mode
2. Extract Java 6 manually (script provided)
3. Replace VUE launcher with shell script wrapper
4. Re-enable SIP if desired
5. Launch VUE successfully

## 🚧 Roadmap
- [ ] Automate detection of `.vue` files and offer migration tools
- [ ] Create a signed wrapper `.app` to avoid Gatekeeper entirely
- [ ] Patch Quaqua dependencies (libquaqua64)
- [ ] Offer Homebrew-style install option for patched launcher

## 🛡️ Disclaimer
This repo is for educational and archival use. VUE is no longer maintained, and this project is provided "as-is" to help users recover their intellectual work.

## ❤️ Contribute
If you’re a Java wizard, systems hacker, or former VUE user who wants to help — pull requests (PRs) are welcome.

## 🪦 Long Live the Maps
"Just because they left us behind doesn’t mean we leave our work behind too."

— Dez
