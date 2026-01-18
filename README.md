# Python & Data Science Course

A comprehensive beginner-to-advanced course covering Python fundamentals, NumPy, Matplotlib, Pandas, SciPy, and Boto3 (AWS) for data analysis and scientific computing.

## Course Overview

| Module | Topic | Notebooks |
|--------|-------|-----------|
| 0 | Getting Started | 2 items |
| 1 | Python Fundamentals | 10 notebooks |
| 2 | NumPy | 5 notebooks |
| 3 | Matplotlib | 4 notebooks |
| 4 | Pandas | 6 notebooks |
| 5 | SciPy | 4 notebooks |
| 6 | Boto3/AWS | 4 notebooks |
| 7 | Capstone Projects | 3 notebooks |

**Total: 38 items** (1 markdown guide + 37 notebooks)

## Prerequisites

- No prior programming experience required for Module 1
- Basic Python knowledge required for Modules 2-7
- AWS account required for Module 6 (free tier sufficient)

## Installation

See [00_getting_started/00_installation_guide.md](00_getting_started/00_installation_guide.md) for detailed setup instructions.

**Quick Start (Anaconda recommended):**
```bash
# Install Anaconda from https://www.anaconda.com/download

# Create environment
conda create -n datasci python=3.11

# Activate environment
conda activate datasci

# Install packages
conda install numpy pandas matplotlib scipy jupyter
pip install boto3
```

## Course Structure

### Module 0: Getting Started
- Installation Guide - Setting up Python, Jupyter, and required packages
- Jupyter Notebook Basics - Cells, markdown, running code, shortcuts

### Module 1: Python Fundamentals
1. Variables and Data Types
2. Strings
3. Lists
4. Tuples and Sets
5. Dictionaries
6. Control Flow
7. Loops
8. Functions
9. File I/O and Exceptions
10. Classes and Objects

### Module 2: NumPy
1. Array Fundamentals
2. Indexing and Slicing
3. Array Operations
4. Broadcasting and Vectorization
5. Linear Algebra and Random

### Module 3: Matplotlib
1. Plotting Basics
2. Plot Types
3. Customization
4. Subplots and Layouts

### Module 4: Pandas
1. Series and DataFrames
2. Reading and Writing Data
3. Indexing and Selection
4. Data Cleaning
5. Groupby and Aggregation
6. Merging and Joining

### Module 5: SciPy
1. Statistics
2. Interpolation and Fitting
3. Optimization
4. Integration and ODEs

### Module 6: Boto3/AWS
1. AWS Fundamentals and Setup
2. S3 Operations
3. Working with Other Services
4. Practical Patterns

### Module 7: Capstone Projects
1. Data Analysis Project
2. Scientific Computing Project
3. Cloud Data Pipeline

## Notebook Structure

Each notebook follows a consistent format:

1. **Learning Objectives** - What you'll learn
2. **Concepts** - Explanations with examples
3. **Exercises** - Practice problems (3-5 per notebook)
4. **Solutions** - Collapsed/hidden solutions
5. **Summary** - Key takeaways

## Directory Structure

```
python_learning/
├── README.md
├── 00_getting_started/
│   ├── 00_installation_guide.md
│   └── 01_jupyter_basics.ipynb
├── 01_python_fundamentals/
│   ├── 01_variables_and_types.ipynb
│   ├── 02_strings.ipynb
│   └── ... (10 notebooks)
├── 02_numpy/
│   └── ... (5 notebooks)
├── 03_matplotlib/
│   └── ... (4 notebooks)
├── 04_pandas/
│   └── ... (6 notebooks)
├── 05_scipy/
│   └── ... (4 notebooks)
├── 06_boto3/
│   └── ... (4 notebooks)
├── 07_capstone/
│   └── ... (3 notebooks)
└── data/
    └── (sample datasets for exercises)
```

## How to Use This Course

1. **Start from Module 0** if you're new to Python/Jupyter
2. **Work through notebooks sequentially** - concepts build on each other
3. **Run all code cells** - type them yourself for better retention
4. **Complete the exercises** - check solutions only after attempting
5. **Build the capstone projects** - apply your skills to real problems

## License

This course material is provided for educational purposes.
