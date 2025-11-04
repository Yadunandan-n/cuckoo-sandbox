Cuckoo Sandbox — Dynamic Malware Analysis Framework

Overview

This project demonstrates the deployment and customization of **Cuckoo Sandbox** for dynamic malware analysis.  
It automates the execution of suspicious files in an isolated environment and captures their behavioral patterns — such as file operations, registry changes, and network activity.  

The repository is designed for **academic research and cybersecurity training**, enabling safe experimentation with real or simulated malware samples.

---

Repository Structure

| File / Folder | Description |
|----------------|-------------|
| `install.sh` | Automates environment setup and dependency installation |
| `conf/cuckoo.conf` | Core configuration for sandbox and database connection |
| `modules/processing/custom_analysis.py` | Custom Python module for result analysis |
| `modules/signatures/custom_signature.py` | Signature rule for detecting suspicious API activity |
| `scripts/setup_db.sh` | Helper script for initializing SQLite database |
| `examples/tasks/sample_task.json` | Example file for task submission |
| `README.md` | Documentation for setup and execution |

---

 System Requirements

- **Operating System:** Ubuntu 20.04+ or any Debian-based distribution  
- **Python:** Version 3.10 or higher  
- **Database:** SQLite (default) or PostgreSQL  
- **Additional Tools:** Virtualenv / venv, Git, and build-essential libraries

---

 Installation Steps

```bash
# Clone the repository
git clone https://github.com/<your-username>/cuckoo-sandbox-project.git
cd cuckoo-sandbox-project

# Make the setup script executable
chmod +x install.sh

# Run installation
./install.sh

# Activate the virtual environment
source venv/bin/activate

# Initialize the database
./scripts/setup_db.sh
