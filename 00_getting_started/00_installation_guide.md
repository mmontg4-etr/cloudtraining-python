# Installation Guide

This guide walks you through setting up Python and Jupyter for this course.

---

## Option 1: GitHub Codespaces (Recommended)

GitHub Codespaces provides a complete, pre-configured development environment in your browser. No local installation required.

### Step 1: Open the Repository in Codespaces

1. Go to the repository: [cloudtraining-python](https://github.com/mmontg4-etr/cloudtraining-python)
2. Click the green **Code** button
3. Select the **Codespaces** tab
4. Click **Create codespace on main**

### Step 2: Wait for Environment Setup

The codespace will automatically:
- Set up a Python environment
- Install required packages
- Configure Jupyter

This takes 1-2 minutes on first launch.

### Step 3: Open Notebooks

Once ready, you can:
- Open `.ipynb` files directly (VS Code's Jupyter extension is pre-installed)
- Or run `jupyter notebook` in the terminal for the classic interface

### Benefits of Codespaces

- **Zero setup** - Everything is pre-configured
- **Consistent environment** - Same setup for everyone
- **Cloud-based** - Work from any device with a browser
- **Free tier available** - 60 hours/month for free GitHub accounts

---

## Option 2: Local Installation (Python + pip)

Install Python and packages locally on your machine.

### Step 1: Install Python

**Windows:**
1. Go to [python.org/downloads](https://www.python.org/downloads/)
2. Download Python 3.11 or later
3. Run the installer
4. **Important:** Check "Add Python to PATH" during installation

**macOS:**
```bash
# Using Homebrew (recommended)
brew install python@3.11

# Or download from python.org
```

**Linux (Ubuntu/Debian):**
```bash
sudo apt update
sudo apt install python3.11 python3.11-venv python3-pip
```

### Step 2: Verify Python Installation

Open a terminal and run:
```bash
python --version
# or on some systems:
python3 --version
```

You should see `Python 3.11.x` or later.

### Step 3: Create a Virtual Environment

Creating a virtual environment keeps your course packages isolated:

```bash
# Navigate to where you want the project
cd ~/projects

# Clone the repository
git clone https://github.com/mmontg4-etr/cloudtraining-python.git
cd cloudtraining-python

# Create virtual environment
python -m venv venv

# Activate (Windows Command Prompt)
venv\Scripts\activate

# Activate (Windows PowerShell)
venv\Scripts\Activate.ps1

# Activate (macOS/Linux)
source venv/bin/activate
```

When activated, you'll see `(venv)` at the start of your terminal prompt.

### Step 4: Install Required Packages

```bash
pip install numpy pandas matplotlib scipy jupyter boto3
```

### Step 5: Launch Jupyter

```bash
jupyter notebook
```

This will open Jupyter in your default web browser.

---

## Required Packages Summary

| Package | Version | Purpose |
|---------|---------|---------|
| Python | 3.10+ | Programming language |
| NumPy | 1.20+ | Numerical computing |
| Pandas | 1.3+ | Data manipulation |
| Matplotlib | 3.4+ | Visualization |
| SciPy | 1.7+ | Scientific computing |
| Jupyter | Latest | Interactive notebooks |
| boto3 | Latest | AWS SDK |

### Installing Additional Packages

```bash
# Always activate your environment first
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install with pip
pip install package_name
```

---

## Verifying Your Setup

Run the following in a Jupyter notebook or Python interpreter:

```python
import sys
print(f"Python: {sys.version}")

import numpy as np
print(f"NumPy: {np.__version__}")

import pandas as pd
print(f"Pandas: {pd.__version__}")

import matplotlib
print(f"Matplotlib: {matplotlib.__version__}")

import scipy
print(f"SciPy: {scipy.__version__}")

import boto3
print(f"boto3: {boto3.__version__}")

print("\nAll packages installed successfully!")
```

---

## Troubleshooting

### "python not found" error
- Ensure Python is added to your PATH
- Try `python3` instead of `python`
- Windows: Reinstall Python and check "Add Python to PATH"

### "pip not found" error
- Try `python -m pip` instead of `pip`
- Or `python3 -m pip` on some systems

### Virtual environment won't activate (PowerShell)
- Run: `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`
- Then try activating again

### Package import errors
- Ensure your virtual environment is activated (look for `(venv)` in prompt)
- Reinstall the package: `pip install package_name`

### Jupyter won't start
- Check if Jupyter is installed: `jupyter --version`
- Reinstall: `pip install jupyter`

### Permission errors
- Windows: Run terminal as Administrator
- Mac/Linux: Don't use `sudo` with pip in a virtual environment

---

## IDE Options

While this course uses Jupyter notebooks, you can also use:

- **VS Code** - Install the Python and Jupyter extensions (recommended)
- **PyCharm** - Full-featured Python IDE with Jupyter support
- **JupyterLab** - Enhanced Jupyter interface: `pip install jupyterlab` then `jupyter lab`

---

## Next Steps

Once your environment is set up, proceed to:
- [01_jupyter_basics.ipynb](01_jupyter_basics.ipynb) - Learn to use Jupyter notebooks
