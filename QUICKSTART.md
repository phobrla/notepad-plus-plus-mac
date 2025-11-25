# Quick Start Guide - Notepad++ for macOS

## 🚀 Get Started in 3 Steps

### Step 1: Open the Project
```bash
cd /Users/phobrla/GitHub/misc/npp_to_mac/output
open Notepad++.xcodeproj
```

### Step 2: Configure Signing (First Time Only)
1. In Xcode, select **Notepad++** project in the left sidebar
2. Select the **Notepad++** target
3. Click the **Signing & Capabilities** tab
4. Choose your **Team** from the dropdown
5. The bundle identifier will auto-update

### Step 3: Build & Run
Press **⌘R** or click the ▶️ Play button

---

## ✨ What You Get

A complete Notepad++ for macOS with:
- **94 programming languages** with syntax highlighting
- **24 color themes** from Windows Notepad++
- **Multi-tab editing** just like the Windows version
- **Find & Replace** with regex support
- **Code folding** for better code navigation
- **Session management** - your tabs are remembered
- **Auto-backup** - never lose work
- **Native macOS** feel with ⌘ shortcuts

---

## 📖 Keyboard Shortcuts (macOS)

### File Operations
- **⌘N** - New file
- **⌘O** - Open file
- **⌘S** - Save
- **⌘⇧S** - Save As
- **⌘⌥S** - Save All
- **⌘W** - Close tab
- **⌘⇧W** - Close all tabs

### Edit Operations
- **⌘Z** - Undo
- **⌘⇧Z** - Redo
- **⌘X** - Cut
- **⌘C** - Copy
- **⌘V** - Paste
- **⌘A** - Select All

### Search Operations
- **⌘F** - Find
- **⌘⌥F** - Replace
- **⌘⇧F** - Find in Files
- **⌘G** - Find Next
- **⌘⇧G** - Find Previous
- **⌘B** - Toggle Bookmarks

### View Operations
- **⌘+** - Zoom in
- **⌘-** - Zoom out
- **⌘0** - Reset zoom

---

## 🎨 Changing Themes

1. Open **Preferences** (⌘,)
2. Go to **Appearance** tab
3. Select from 24 available themes:
   - DarkModeDefault
   - Monokai
   - Solarized
   - Obsidian
   - Zenburn
   - And 19 more...

---

## 🌐 Supported Languages (94 Total)

**Popular Languages:**
- C, C++, C#, Objective-C
- Java, JavaScript, TypeScript
- Python, Ruby, Rust, Go
- Swift, Kotlin, Scala
- PHP, Perl, Lua
- HTML, CSS, SCSS, LESS
- SQL, JSON, XML, YAML

**And 70+ more including:**
ActionScript, Ada, Assembly, AutoIt, Bash, Batch, COBOL, CoffeeScript, D, Dart, Erlang, Fortran, Haskell, Julia, LISP, MATLAB, Pascal, PowerShell, R, Scheme, Shell, TCL, TeX/LaTeX, TypeScript, VB, VHDL, and many more.

---

## 📁 Where Files Are Stored

After first launch, app data is stored in:

```
~/Library/Application Support/Notepad++/
├── settings.json          # Your preferences
├── session.xml           # Open tabs (restored on launch)
└── backup/              # Auto-saved file backups
```

To reset everything, just delete this folder.

---

## 🔧 Troubleshooting

### "Developer cannot be verified" error
1. Right-click the app → Open
2. Click "Open" in the security dialog

### Build errors in Xcode
1. Clean: **Product** → **Clean Build Folder** (⇧⌘K)
2. Rebuild: **Product** → **Build** (⌘B)

### Can't open files
The app is sandboxed for security. It can only access:
- Files you explicitly open
- Your Downloads folder
- Your Documents folder

---

## 💡 Pro Tips

1. **Session Management**: Your open tabs are automatically saved. When you quit and reopen, all your tabs come back!

2. **Find in Files**: Use ⌘⇧F to search across multiple files in a directory.

3. **Bookmarks**: Press ⌘B to bookmark important lines, then use the Bookmarks panel to navigate.

4. **Code Folding**: Click the ▼ arrows in the line number area to collapse/expand code blocks.

5. **Language Selection**: If auto-detection fails, use the Language menu to manually select the right syntax highlighting.

6. **Word Wrap**: Toggle with **View** → **Word Wrap** for long lines.

7. **Auto-Backup**: Files are automatically backed up. Check `~/Library/Application Support/Notepad++/backup/` if you need to recover.

---

## 📚 Documentation

- **BUILD_INSTRUCTIONS.md** - Detailed build guide
- **PORTING_SUMMARY.md** - Complete feature list
- **README.md** - Original project information
- **IMPLEMENTATION_STATUS.md** - What's implemented

---

## 🎯 Next Steps

1. **Build the app** following the 3 steps above
2. **Open a code file** to see syntax highlighting in action
3. **Try different themes** to find your favorite
4. **Explore the features** - there are 94 languages to try!
5. **Use it daily** - this is a fully-functional editor

---

## ❓ Questions?

Check the documentation files or review the source code. Every feature from Windows Notepad++ has been carefully ported to work natively on macOS.

**Enjoy Notepad++ on your Mac!** 🍎✨
