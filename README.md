# 🟢 GreenEye - Lightweight Antivirus & File Activity Monitor (Ongoing Project)

**GreenEye** is a lightweight, script-based antivirus and file activity monitor designed for controlled environments such as testing labs and developer workstations. Originally built in **November 2023**, it includes core monitoring capabilities with options to automatically delete suspicious files, shut down the system, or alert on webcam activity.

> ⚠️ This is an **ongoing project** that is currently on hold. It is **not intended for full-time use**, but rather for **temporary deployment during debugging or controlled testing sessions**.

---

## 👁️ Key Features

- 🔍 **Directory Monitoring** – Watches a specific path for new file creation  
- ❌ **Optional Auto-Deletion** – Removes unauthorized files on creation  
- 📴 **Emergency Shutdown** – Shuts down the PC if flagged  
- 🧾 **Audit & Ownership Checks** – Retrieves owner and file audit data  
- 🎥 **Webcam Usage Detection** – Alerts if the camera appears to be in use  
- 🎨 **Stylized ASCII Interface** – Displays themed intro banners  

---

## 📁 Setup & Usage

### 1. Clone the Repository

```bash
git clone https://github.com/CecuTheMag/GreenEye
cd GreenEye
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure Monitoring

Edit `config.json` to set your desired behavior:

```json
{
  "turn_off_pc": "T",
  "delete_new_files": "F",
  "path_to_monitor": "C:\\Users\\YourName\\Desktop\\WatchThis",
  "check_for_cam_spy": "T"
}
```

| Key                 | Description                              | Options     |
|---------------------|------------------------------------------|-------------|
| `turn_off_pc`       | Shut down PC when file is created        | `"T"` / `"F"` |
| `delete_new_files`  | Delete suspicious new files              | `"T"` / `"F"` |
| `path_to_monitor`   | Folder to watch for file activity        | Absolute path |
| `check_for_cam_spy` | Alert when webcam usage is detected      | `"T"` / `"F"` |

### 4. Run the Script

```bash
python greeneye.py
```

A themed ASCII banner will appear, followed by active real-time monitoring of the folder and system status.

---
![GreenEye Eye](eye.png)
---

## 🗂️ Project Structure

```
GreenEye/
├── greeneye.py         # Main antivirus monitor script
├── config.json         # Runtime configuration
├── requirements.txt    # Python dependencies
├── eye.png             # Logo / preview image
└── README.md           # Documentation
```

---

## ⚠️ Legal & Ethical Disclaimer

GreenEye is intended **only for use in environments where you have full control and permission**. This script is a proof-of-concept and:

- ❌ Is **not a replacement** for full antivirus suites  
- ✅ Should be used only in **lab/testing/dev environments**  
- ⚠️ Must **not** be used for unauthorized monitoring or data collection  

You are responsible for how you use this tool. Use responsibly.

---

## 📊 Project Status

- ✅ Concept complete  
- 🚧 Paused – development suspended as of mid-2024  
- 🧪 Still useful in test workflows or personal system experiments  

---

## 🧑‍💻 Author

**MagCecu**  
Originally developed in **November 2023**  
