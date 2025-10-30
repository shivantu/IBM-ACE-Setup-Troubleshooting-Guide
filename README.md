# 🚀 IBM ACE (App Connect Enterprise) – Setup & Troubleshooting Guide

This repository contains installation steps, configuration tips, and troubleshooting solutions for IBM App Connect Enterprise (ACE) running on Linux environments.

---
© 2025 Shivaraj — All Rights Reserved.  

---

## 📦 What’s Inside?

| Category | Includes |
|---------|----------|
| 🔧 Installation | Linux installation steps (Refer IBM Docs) |
| ⚙️ Configuration | Node & Integration Server setup |
| 🧩 Connectivity | MQ connectivity setup |
| 🔐 Deployment | Application Deplyment and status check |
| 🏥 Troubleshooting | Common errors + solutions |
| 📝 Commands | Admin & debug commands |

---

## ✅ IBM ACE Linux Installation (Latest Version)

### Steps Summary
```bash
# 1. Log in as root or as user with appropriate permissions
#    For shared install, root or a user with write access to /var/mqsi

# 2. Navigate to directory where you will unpack
cd /opt/IBM
tar -xzvf ace-13.0.4.0.tar.gz            # example version 13.0.4.0  
# If you want to exclude unnecessary components:
tar -xzvf ace-13.0.4.0.tar.gz --exclude ace-13.0.4.0/server/wsrrcomponent --exclude ace-13.0.4.0/tools  # optional  

# 3. Change to installation directory
cd ace-13.0.4.0

# 4. Accept license
# - Single user install:
./ace accept license
# or silently:
./ace accept license silently

# - Shared install:
./ace make registry global accept license
# or silently:
./ace make registry global accept license silently

# 5. (Optional) Create work directory
# For shared install, a registry is created in /var/mqsi (default)
```

## 📞 Contact
- shivaraj
- shivantu9@gmail.com
- For questions or contributions, please reach out via GitHub issues.

---
