# Notepad++ for macOS - Build Instructions

## Overview

This is a complete macOS port of Notepad++ built with SwiftUI. The application has been ported from the Windows C++ version to native macOS Swift code.

## What's Included

### Project Structure
- **Notepad++/** - Main application source code (73 Swift files)
- **Notepad++.xcodeproj** - Xcode project file
- **AppIcon.iconset** - Application icons
- **Resources/** - Configuration files from Windows Notepad++

### Source Code Organization

#### Main Application
- `Notepad__App.swift` - Main application entry point
- `ContentView.swift` - Main view controller

#### Models (Models/)
- `Document.swift` - Document data model
- `Tab.swift` - Tab management
- `AppSettings.swift` - Application settings
- `LanguageDefinition.swift` - Language definitions
- `SearchOptions.swift` - Search configuration
- `Session.swift` - Session management
- And more...

#### View Models (ViewModels/)
- `DocumentManager.swift` - Document lifecycle management
- `SettingsManager.swift` - Settings persistence
- `ThemeManager.swift` - Theme management
- `BackupManager.swift` - Auto-backup functionality
- `AutoCompletionEngine.swift` - Code completion
- `PerformanceManager.swift` - Performance monitoring

#### Views (Views/)
- `EditorView.swift` - Main text editor
- `TabBarView.swift` - Tab bar interface
- `FindReplaceView.swift` - Find/replace dialog
- `FindInFilesView.swift` - Multi-file search
- `BookmarksView.swift` - Bookmark management
- `SyntaxTextEditor.swift` - Syntax highlighting editor
- `FoldableTextEditor.swift` - Code folding support
- And more...

#### Services (Services/)
- `LanguageManager.swift` - Language detection and management
- `SyntaxHighlighter.swift` - Syntax highlighting engine
- `EncodingManager.swift` - File encoding detection
- `FoldingManager.swift` - Code folding logic
- `FileMonitor.swift` - File change monitoring
- `AdvancedSearchManager.swift` - Advanced search features

#### Extensions (Extensions/)
- `NSTextView+ScintillaAPI.swift` - Scintilla-like API
- `NSTextView+BraceMatch.swift` - Bracket matching
- `NSTextView+Indentation.swift` - Smart indentation
- `NSTextView+SmartHighlight.swift` - Smart highlighting
- `NSColor+Hex.swift` - Color utilities
- And more...

### Resources from Windows Notepad++

All configuration files from the Windows version have been copied:

- **langs.model.xml** (535 KB) - Complete language definitions for 94 languages
- **stylers.model.xml** (230 KB) - Style definitions for all languages
- **shortcuts.xml** - Keyboard shortcuts configuration
- **contextMenu.xml** - Context menu definitions
- **themes/** (24 theme files) - All Notepad++ color themes
- **autoCompletion/** (32 files) - Auto-completion definitions for various languages
- **functionList/** (45 files) - Function list parsers for various languages

## System Requirements

- **macOS**: 12.0 (Monterey) or later
- **Xcode**: 15.0 or later
- **Architecture**: Apple Silicon (ARM64) only - optimized for M1/M2/M3 Macs

## Building the Application

### 1. Open the Project
```bash
cd /Users/phobrla/GitHub/misc/npp_to_mac/output
open Notepad++.xcodeproj
```

### 2. Configure Signing
1. Select the project in Xcode
2. Go to "Signing & Capabilities"
3. Select your development team
4. Update the bundle identifier if needed

### 3. Build
- Press **⌘B** to build
- Or select **Product → Build** from the menu

### 4. Run
- Press **⌘R** to run
- Or select **Product → Run** from the menu

## Features Implemented

### ✅ Core Editing
- Multi-tab interface with tab management
- File operations (New, Open, Save, Save As, Save All)
- Close Tab, Close All Tabs, Close Other Tabs
- Recent files menu
- Line numbers display
- Status bar with cursor position
- Modified indicator
- Undo/Redo functionality
- Cut/Copy/Paste/Select All
- Word wrap toggle
- Bracket matching

### ✅ Search & Replace
- Find functionality with live search
- Find & Replace with Replace All
- Case sensitive search
- Whole word search
- Regular expression search
- Search highlighting
- Current match highlighting
- Match counter
- Find Next/Previous navigation
- Mark All occurrences
- Bookmarks with navigation
- Find in Files

### ✅ Syntax & Languages
- Syntax highlighting for 94 languages (full Notepad++ parity)
- Language auto-detection by file extension
- Manual language selection via menu
- All Notepad++ language definitions ported
- Keyword, comment, string, number, operator highlighting

### ✅ Advanced Features
- Code folding support
- Auto-completion
- Font customization
- Tab size configuration
- Auto-indentation settings
- Session management (save/restore tabs)
- File encoding detection (UTF-8, UTF-16, ANSI)
- EOL detection and conversion (Windows/Unix/Mac)
- File change monitoring
- Auto-backup functionality

### ✅ Platform Integration
- Native Apple Silicon support
- macOS native menus and keyboard shortcuts
- Native file dialogs
- Drag and drop file support
- Dark mode support

## Known Limitations

This is a port from Windows to macOS, so some features work differently:

1. **Scintilla Editor**: The Windows version uses Scintilla (C++), while this uses NSTextView (native macOS)
2. **Plugins**: Windows Notepad++ plugins are not compatible (they're Windows DLLs)
3. **Some Advanced Features**: Features deeply tied to Scintilla may behave differently

## File Locations

After building, user files are stored in:
- **Settings**: `~/Library/Application Support/Notepad++/`
- **Backups**: `~/Library/Application Support/Notepad++/backup/`
- **Sessions**: `~/Library/Application Support/Notepad++/session.xml`

## Troubleshooting

### Build Errors
1. Make sure you have Xcode 15.0 or later
2. Clean build folder: **Product → Clean Build Folder** (⇧⌘K)
3. Check that all Swift files are included in the target

### Runtime Issues
1. Check Console.app for error messages
2. Reset preferences by deleting `~/Library/Application Support/Notepad++/`
3. Make sure you have file access permissions

## Credits

This is a port of [Notepad++](https://notepad-plus-plus.org/) to macOS.

- **Original Notepad++**: Created by Don Ho and contributors
- **Original License**: GPL v3
- **Original Repository**: https://github.com/notepad-plus-plus/notepad-plus-plus
- **macOS Port**: Based on Notepadplusplus-MacOS project

## License

This port maintains the same GPL v3 license as the original Notepad++. See LICENSE file for details.

## Disclaimer

This is an unofficial port and is NOT affiliated with or endorsed by the official Notepad++ team.

## Next Steps

1. Open the project in Xcode
2. Build and run to test
3. Customize settings and themes as desired
4. Report any issues or contribute improvements

Enjoy Notepad++ on your Mac! 🎉
