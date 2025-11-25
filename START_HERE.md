# 📖 Notepad++ for macOS - Documentation Index

Welcome! This is your complete guide to the Notepad++ macOS port.

---

## 🚀 Getting Started (Start Here!)

**→ [QUICKSTART.md](QUICKSTART.md)** - Build and run in 3 steps  
Perfect for: I just want to use Notepad++ on my Mac right now!

---

## 📚 Documentation Files

### For Users

**[README.md](README.md)**  
Original project overview and background information about the port.

**[QUICKSTART.md](QUICKSTART.md)**  
Quick 3-step guide to build and run the app. Includes keyboard shortcuts and pro tips.

**[BUILD_INSTRUCTIONS.md](BUILD_INSTRUCTIONS.md)**  
Detailed build instructions, system requirements, troubleshooting, and feature list.

### For Developers

**[PORTING_SUMMARY.md](PORTING_SUMMARY.md)**  
Complete overview of what was ported: 73 Swift files, 104 resources, all features documented.

**[IMPLEMENTATION_STATUS.md](IMPLEMENTATION_STATUS.md)**  
Detailed status of every feature - what's working, what's in progress, what's planned.

**[PORTING_NOTES.md](PORTING_NOTES.md)**  
Technical notes about the porting process from Windows C++ to macOS Swift.

**[CONTRIBUTING.md](CONTRIBUTING.md)**  
How to contribute to the project.

**[CLAUDE.md](CLAUDE.md)**  
Notes about AI-assisted development.

**[NEXT_FEATURES.md](NEXT_FEATURES.md)**  
Planned features and enhancements.

### Legal

**[LICENSE](LICENSE)**  
GPL v3 license (same as original Notepad++)

---

## 📂 What's In This Project?

```
output/
├── 📖 Documentation (you are here)
│   ├── QUICKSTART.md              ← Start here!
│   ├── BUILD_INSTRUCTIONS.md      ← Detailed build guide
│   ├── PORTING_SUMMARY.md         ← What was ported
│   ├── README.md                  ← Project overview
│   └── ... more docs
│
├── 💻 Application Source Code
│   └── Notepad++/
│       ├── Notepad__App.swift     ← Main app
│       ├── ContentView.swift      ← Main view
│       ├── Models/                ← 13 data models
│       ├── ViewModels/            ← 6 view models
│       ├── Views/                 ← 20+ UI components
│       ├── Services/              ← 9 core services
│       ├── Extensions/            ← 11 extensions
│       └── Resources/             ← 104 config files
│           ├── langs.model.xml    ← 94 languages
│           ├── themes/            ← 24 themes
│           ├── autoCompletion/    ← 32 languages
│           └── functionList/      ← 45 parsers
│
└── 🔧 Project Files
    ├── Notepad++.xcodeproj/       ← Xcode project
    └── AppIcon.iconset/           ← App icons
```

**Total:** 73 Swift files, 104 resource files, ~10 MB

---

## 🎯 Quick Navigation

### I want to...

**...build the app right now**  
→ [QUICKSTART.md](QUICKSTART.md) - 3 steps, you'll be running in minutes

**...understand what features are included**  
→ [BUILD_INSTRUCTIONS.md](BUILD_INSTRUCTIONS.md#features-implemented) - Complete feature checklist

**...see all 94 supported languages**  
→ [QUICKSTART.md](QUICKSTART.md#-supported-languages-94-total) - Full language list

**...know what was ported from Windows**  
→ [PORTING_SUMMARY.md](PORTING_SUMMARY.md) - Complete porting details

**...understand the code structure**  
→ [PORTING_SUMMARY.md](PORTING_SUMMARY.md#-core-components) - Detailed file breakdown

**...contribute or modify the code**  
→ [CONTRIBUTING.md](CONTRIBUTING.md) - Contribution guidelines

**...troubleshoot build issues**  
→ [BUILD_INSTRUCTIONS.md](BUILD_INSTRUCTIONS.md#troubleshooting) - Common fixes

**...see what's planned next**  
→ [NEXT_FEATURES.md](NEXT_FEATURES.md) - Roadmap

---

## ✨ Key Features At A Glance

- ✅ **94 Programming Languages** - Full Notepad++ language support
- ✅ **24 Color Themes** - All Windows themes included
- ✅ **Multi-Tab Interface** - Work on multiple files simultaneously
- ✅ **Advanced Search** - Find & Replace with regex support
- ✅ **Code Folding** - Collapse/expand code blocks
- ✅ **Session Management** - Remembers your open tabs
- ✅ **Auto-Backup** - Never lose your work
- ✅ **Syntax Highlighting** - Real-time, language-aware
- ✅ **Find in Files** - Search across multiple files
- ✅ **Native macOS** - Apple Silicon optimized

---

## 🏗️ Project Stats

| Metric | Count |
|--------|-------|
| Swift Source Files | 73 |
| Resource Files | 104 |
| Supported Languages | 94 |
| Color Themes | 24 |
| Auto-Completion Languages | 32 |
| Function List Parsers | 45 |
| Total Project Size | ~10 MB |
| Lines of Code | ~15,000+ |

---

## 🔗 Useful Links

**Original Notepad++**  
- Website: https://notepad-plus-plus.org/
- GitHub: https://github.com/notepad-plus-plus/notepad-plus-plus

**This Port**  
- Built with: SwiftUI + macOS 12.0+
- Architecture: Apple Silicon (ARM64)
- License: GPL v3

---

## 📞 Support

### Build Issues?
1. Check [BUILD_INSTRUCTIONS.md - Troubleshooting](BUILD_INSTRUCTIONS.md#troubleshooting)
2. Verify you have Xcode 15.0+
3. Clean build folder (⇧⌘K) and rebuild

### Feature Questions?
1. Check [IMPLEMENTATION_STATUS.md](IMPLEMENTATION_STATUS.md) for feature status
2. Review [PORTING_SUMMARY.md](PORTING_SUMMARY.md) for complete feature list

### Want to Contribute?
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines

---

## ⚡ TL;DR - Just Want to Run It?

```bash
cd /Users/phobrla/GitHub/misc/npp_to_mac/output
open Notepad++.xcodeproj
# Then press ⌘R in Xcode
```

That's it! 🎉

---

**Last Updated:** November 19, 2025  
**Version:** 1.0 (Complete macOS port)  
**Status:** ✅ Ready to build and use
