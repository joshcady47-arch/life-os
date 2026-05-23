# Windows → macOS Cheat Sheet 🪟➡️🍎

A quick reference for Josh — everything you already know on Windows, mapped to how it works on Mac.

---

## ⌨️ Keyboard Shortcuts

The biggest change: **`Ctrl` → `Cmd` (⌘)** for almost everything.

| Action | Windows | Mac |
|---|---|---|
| Copy | `Ctrl+C` | `Cmd+C` |
| Paste | `Ctrl+V` | `Cmd+V` |
| Cut | `Ctrl+X` | `Cmd+X` |
| Undo | `Ctrl+Z` | `Cmd+Z` |
| Redo | `Ctrl+Y` | `Cmd+Shift+Z` |
| Save | `Ctrl+S` | `Cmd+S` |
| Select All | `Ctrl+A` | `Cmd+A` |
| Find | `Ctrl+F` | `Cmd+F` |
| New Window/Tab | `Ctrl+N` / `Ctrl+T` | `Cmd+N` / `Cmd+T` |
| Close Window | `Alt+F4` | `Cmd+W` (close tab) / `Cmd+Q` (quit app) |
| Switch Apps | `Alt+Tab` | `Cmd+Tab` |
| Switch Windows (same app) | — | `Cmd+\`` (backtick) |
| Screenshot (full) | `PrtScn` | `Cmd+Shift+3` |
| Screenshot (select area) | `Win+Shift+S` | `Cmd+Shift+4` |
| Lock Screen | `Win+L` | `Cmd+Ctrl+Q` |
| Show Desktop | `Win+D` | `Cmd+F3` or 4-finger spread on trackpad |
| Open Spotlight (like Search) | `Win` key | `Cmd+Space` |
| Force Quit (like Task Manager) | `Ctrl+Alt+Delete` | `Cmd+Option+Esc` |
| Rename file | `F2` | `Enter` (yes, Enter renames on Mac!) |
| Delete file (to Trash) | `Delete` | `Cmd+Delete` |
| Delete permanently | `Shift+Delete` | `Cmd+Option+Delete` |
| Open file | `Enter` | `Cmd+O` or `Cmd+Down Arrow` |
| Go up a folder | `Backspace` | `Cmd+Up Arrow` |
| Home / End (line) | `Home` / `End` | `Cmd+Left` / `Cmd+Right` |
| Top / Bottom of doc | `Ctrl+Home/End` | `Cmd+Up` / `Cmd+Down` |
| Word jump | `Ctrl+Left/Right` | `Option+Left/Right` |

---

## 🗂️ App Equivalents

| Windows | macOS |
|---|---|
| File Explorer | Finder |
| Task Manager | Activity Monitor (`Cmd+Space` → "Activity Monitor") |
| Control Panel / Settings | System Settings (Apple menu → System Settings) |
| Notepad | TextEdit |
| Paint | Preview (basic) |
| Word / Excel | Pages / Numbers (or install Microsoft Office) |
| Windows Defender | Built-in (XProtect) — nothing to manage |
| Regedit | No equivalent (use `defaults` in Terminal) |
| `C:\Users\Josh` | `/Users/joshcady` |
| `C:\Program Files` | `/Applications` |
| Command Prompt | Terminal (or iTerm2) |
| PowerShell | Terminal + zsh |

---

## 🪟 Window Management (The Biggest Miss from Windows)

macOS has **no built-in window snapping**. We installed **Rectangle** to fix this.

| Action | Windows | Rectangle (Mac) |
|---|---|---|
| Snap left half | `Win+Left` | `Ctrl+Option+Left` |
| Snap right half | `Win+Right` | `Ctrl+Option+Right` |
| Maximize | `Win+Up` | `Ctrl+Option+Return` |
| Top half | — | `Ctrl+Option+Up` |
| Bottom half | — | `Ctrl+Option+Down` |
| Full screen | `Win+Up` (twice) | `Ctrl+Cmd+F` |

> **Open Rectangle** from Applications after installing. It lives in your menu bar.

---

## 📁 Finder Tips (File Explorer Equivalent)

- **Show/hide hidden files**: `Cmd+Shift+.` (dot) — toggles instantly
- **Path bar**: View → Show Path Bar (we turned this on for you)
- **Column view**: `Cmd+3` — great for navigating deep folders
- **Quick Look** (preview without opening): Select file → press `Space`
- **Get Info** (like Properties): `Cmd+I`
- **Copy file path**: Right-click → Hold Option → "Copy as Pathname"
- **Open Terminal here**: Right-click folder → New Terminal at Folder

---

## 🖱️ Trackpad Gestures

| Gesture | What it does |
|---|---|
| Two-finger scroll | Scroll (like mouse wheel) |
| Two-finger click | Right-click |
| Two-finger swipe left/right | Go back/forward in browsers |
| Three-finger swipe up | Mission Control (see all windows) |
| Three-finger swipe left/right | Switch between Spaces (virtual desktops) |
| Pinch to zoom | Zoom in/out |
| Four-finger spread | Show Desktop |
| Four-finger pinch | Launchpad (app grid, like Start Menu) |

---

## 💻 Terminal Tips (CMD/PowerShell → zsh)

| Windows | macOS/Linux |
|---|---|
| `dir` | `ls` |
| `cls` | `clear` |
| `copy` | `cp` |
| `move` | `mv` |
| `del` | `rm` |
| `mkdir` | `mkdir` (same) |
| `type file.txt` | `cat file.txt` |
| `where python` | `which python` |
| `ipconfig` | `ifconfig` or `ip addr` |
| `ping` | `ping` (same, but Ctrl+C to stop) |
| `tasklist` | `ps aux` |
| `taskkill` | `kill <PID>` |

---

## 🔧 Things We Already Set Up For You

- ✅ **File extensions always visible** (like Windows default)
- ✅ **Hidden files visible** (`Cmd+Shift+.` to toggle)
- ✅ **Full path shown** in Finder title bar
- ✅ **Folders sorted first** in Finder (like Windows Explorer)
- ✅ **Key repeat enabled** (hold a key and it repeats, no accent popup)
- ✅ **Finder status bar** (shows file count and disk space at bottom)
- ✅ **Rectangle** installed for window snapping

---

## 🆘 Common "Where Did That Go?" Moments

| You're looking for... | Find it here |
|---|---|
| The C: drive | `/` (root) or `/Users/joshcady` for your files |
| Downloads | `/Users/joshcady/Downloads` or Finder sidebar |
| Installed apps | `/Applications` |
| Startup programs | System Settings → General → Login Items |
| Uninstall an app | Drag it from Applications to Trash. Done. |
| Check disk space | Apple Menu → About This Mac → More Info |
| Update macOS | System Settings → General → Software Update |
| Installed fonts | Font Book app |
| Your IP address | System Settings → Network, or `ifconfig en0` in Terminal |

---

> 💡 **Tip for ADHD**: Spotlight (`Cmd+Space`) is your best friend. Don't dig through folders — just type what you want and hit Enter. It finds apps, files, calculator, weather, anything.
