# Installation Guide

This guide walks you through setting up Python and Jupyter for this course.

## Option 1: Anaconda (Recommended for Beginners)

Anaconda is a Python distribution that includes most packages needed for data science.

### Step 1: Download Anaconda

1. Go to [https://www.anaconda.com/download](https://www.anaconda.com/download)
2. Download the installer for your operating system (Windows, macOS, or Linux)
3. Choose Python 3.11 or later

### Step 2: Install Anaconda

**Windows:**
- Run the downloaded `.exe` file
- Follow the installation wizard
- Check "Add Anaconda to PATH" (optional but convenient)

**macOS:**
- Open the downloaded `.pkg` file
- Follow the installation wizard

**Linux:**
```bash
bash Anaconda3-*-Linux-x86_64.sh
```
Follow the prompts and accept the license.

### Step 3: Verify Installation

Open a terminal (or Anaconda Prompt on Windows) and run:
```bash
conda --version
python --version
```

You should see version numbers displayed.

### Step 4: Create a Course Environment (Recommended)

Creating a dedicated environment keeps your course packages isolated:

```bash
# Create environment
conda create -n datasci python=3.11

# Activate environment
conda activate datasci

# Install required packages
conda install numpy pandas matplotlib scipy jupyter

# Install boto3 for AWS module
pip install boto3
```

### Step 5: Launch Jupyter

```bash
# Activate your environment (if not already active)
conda activate datasci

# Launch Jupyter Notebook
jupyter notebook
```

This will open Jupyter in your web browser.

---

## Option 2: pip (For Experienced Users)

If you already have Python installed, you can use pip.

### Step 1: Verify Python Installation

```bash
python --version
```

Ensure you have Python 3.8 or later.

### Step 2: Create a Virtual Environment

```bash
# Create virtual environment
python -m venv datasci

# Activate (Windows)
datasci\Scripts\activate

# Activate (macOS/Linux)
source datasci/bin/activate
```

### Step 3: Install Packages

```bash
pip install numpy pandas matplotlib scipy jupyter boto3
```

### Step 4: Launch Jupyter

```bash
jupyter notebook
```

---

## Required Packages Summary

| Package | Version | Purpose |
|---------|---------|---------|
| Python | 3.8+ | Programming language |
| NumPy | 1.20+ | Numerical computing |
| Pandas | 1.3+ | Data manipulation |
| Matplotlib | 3.4+ | Visualization |
| SciPy | 1.7+ | Scientific computing |
| Jupyter | Latest | Interactive notebooks |
| boto3 | Latest | AWS SDK |

### Installing Additional Packages Later

```bash
# With conda
conda install package_name

# With pip
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

### "conda not found" error
- Windows: Use "Anaconda Prompt" instead of regular command prompt
- Mac/Linux: Run `source ~/.bashrc` or restart your terminal

### "python not found" error
- Ensure Python is added to your PATH
- Try `python3` instead of `python`

### Package import errors
- Ensure your environment is activated: `conda activate datasci`
- Reinstall the package: `conda install package_name`

### Jupyter won't start
- Check if Jupyter is installed: `jupyter --version`
- Reinstall: `conda install jupyter` or `pip install jupyter`

### Permission errors
- Windows: Run terminal as Administrator
- Mac/Linux: Use `sudo` or fix directory permissions

---

## IDE Alternatives (Optional)

While this course uses Jupyter notebooks, you can also use:

- **VS Code** - Install the Python and Jupyter extensions
- **PyCharm** - Full-featured Python IDE
- **JupyterLab** - Next-generation Jupyter interface (`jupyter lab`)

---

## Next Steps

Once your environment is set up, proceed to:
- [01_jupyter_basics.ipynb](01_jupyter_basics.ipynb) - Learn to use Jupyter notebooks
