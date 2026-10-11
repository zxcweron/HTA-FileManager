# HTA File Manager

A lightweight file manager for Windows that **requires no installation**. One `.hta` file — download it, double-click, done.

An alternative to Windows Explorer with tabs, fast folder browsing, and launching programs straight from the list.

## ✨ Features

- **Browser-style tabs** — open multiple folders at once, each keeps its own history
- **Navigation** — back, forward, up one level, refresh, jump to a typed path
- **File list** — name, type, size, modified date. Folders first, files below
- **Launch programs** — double-click an `.exe`, `.bat`, or document to open it with the default app
- **Archive viewing** — double-click a `.zip`, `.tar`, `.gz` to extract it to a temp folder and open it
- **Hotkeys**:
  - `ESC` — close
  - `Backspace` — go up one level
  - `F5` — refresh

## 🚀 How to run

1. Download `file-manager.hta` from this repository
2. Double-click it
3. Done — no installation needed

**Requirements:** Windows 10 or 11. Everything else is already built into the system.

## 📁 Usage

- **Double-click a folder** — enter it
- **Double-click a file** — open it with the default program
- **Double-click an archive** — extract to a temp folder and open it
- **`+` button** — new tab
- **`×` on a tab** — close the tab
- **Path field** — type a path, press `Enter`

## ⚠️ Known limitations

- Archive viewing means **extracting to `%TEMP%`**, not browsing inside the archive like WinRAR does. Temp files may be cleaned up after a reboot.
- Windows only (HTA is a Microsoft technology).
- No copy/paste/delete yet.

## 🛠️ Tech stack

- HTA (HTML Application)
- JScript + ActiveX (`Scripting.FileSystemObject`, `WScript.Shell`)
- Windows built-in `tar` for archive extraction

No Node.js, no Python, no compilers, no installers.

## 🗺️ Roadmap

- [ ] Right-click context menu (copy, paste, delete, rename)
- [ ] Search in current folder
- [ ] Sort by columns
- [ ] Favorite folders
- [ ] Dark theme

## 📜 License

MIT — do whatever you want, just keep the author credit. See [LICENSE](LICENSE).
