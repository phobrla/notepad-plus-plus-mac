# Reference Materials

This directory contains reference implementations and original Notepad++ configurations used during the macOS port development.

## Contents

### Notepadplusplus-MacOS/
Early attempt at a macOS port using different approaches.

### notepadqq/
Linux Qt-based port of Notepad++ (version 1.x) - used as reference for cross-platform implementation patterns.

### notepadqq-2.0.0-beta/
Beta version of the Linux port with updated Qt frameworks.

### npp_to_mac/
The original Windows Notepad++ installation files and user configuration, used as the source for:
- XML configuration schemas (langs.xml, stylers.xml, functionList/*.xml, autoCompletion/*.xml)
- Theme definitions
- Language syntax definitions
- Keyboard shortcut mappings

## Usage

These materials are kept for reference only. The actual Swift/SwiftUI implementation in the project root is independent but uses similar XML schemas and feature sets.
