# Multi-Platform PDF Organizer

A cross-platform Python automation script that scans your system for PDF files and organizes them into a centralized location.

## 📋 Features

* **Cross-Platform**: Runs natively on Windows, macOS, and Linux.
* **Automatic Creation**: Generates missing target folders automatically.
* **Error Prevention**: Skips duplicate files safely without crashing out.
* **Deep Scanning**: Searches recursively through deeply nested folders.

## 🛠️ Requirements

* **Python 3.6+**
* **Built-in libraries only**
* **No external packages needed**
* **Cross-platform compatibility**

## 📥 Command Line Python Installation

If Python is not yet installed on your system, open your terminal and run the appropriate commands:

### Windows (PowerShell)
```powershell
winget source update
winget install Python.Python.3 --scope machine
# Restart PowerShell after installation completes
```

### macOS (Terminal)
```bash
brew update
brew install python
```

### Linux (Ubuntu / Debian Terminal)
```bash
sudo apt update
sudo apt install python3 python3-pip -y
```

## 💻 How to Run It

### Windows
1. Open **PowerShell** or Command Prompt.
2. Run the automation script:
   ```powershell
   python main.py
   ```

### macOS & Linux
1. Open your **Terminal**.
2. Run the automation script:
   ```bash
   python3 main.py
   ```

## 📂 Folder Paths Handled

* **Source Directory**: Looks inside your profile's `Downloads/` directory.
* **Destination Directory**: Migrates discovered files into your `Documents/` directory.

## 🛠️ Built With

* **Pathlib**: Handles cross-platform system path resolutions dynamically.
* **OS**: Powers the structural directory traversal framework (`os.walk`).
* **Shutil**: Processes raw physical file streams and migrations securely.
