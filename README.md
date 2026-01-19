# Python & Data Science Course

A comprehensive beginner-to-advanced course covering Python fundamentals, NumPy, Matplotlib, Pandas, SciPy, SQL, Django, and Boto3 (AWS) for data analysis, web development, and scientific computing.

## Course Overview

| Module | Topic | Notebooks | Test |
|--------|-------|-----------|------|
| 0 | Getting Started | 2 items | - |
| 1 | Python Fundamentals | 10 notebooks | 20 questions |
| 2 | NumPy | 5 notebooks | 15 questions |
| 3 | Matplotlib | 4 notebooks | 12 questions |
| 4 | Pandas | 6 notebooks | 17 questions |
| 5 | SciPy | 4 notebooks | 12 questions |
| 6 | Boto3/AWS | 4 notebooks | 12 questions |
| 7 | SQL in Python | 4 notebooks | 14 questions |
| 8 | Django | 5 notebooks | 15 questions |
| 99 | Capstone Projects | 6 notebooks | - |

**Total: 50 learning items** (1 markdown guide + 49 notebooks) + **8 comprehensive tests**

## Prerequisites

- No prior programming experience required for Module 1
- Basic Python knowledge required for Modules 2-8
- AWS account required for Module 6 (free tier sufficient)

## Getting Started

### Option 1: GitHub Codespaces (Recommended)

The fastest way to start - no local installation required:

1. Click the green **Code** button above
2. Select the **Codespaces** tab
3. Click **Create codespace on main**
4. Wait 1-2 minutes for the environment to build
5. Open any `.ipynb` file to begin

### Option 2: Local Installation (Python + pip)

```bash
# Clone the repository
git clone https://github.com/mmontg4-etr/cloudtraining-python.git
cd cloudtraining-python

# Create virtual environment
python -m venv venv

# Activate (Windows)
venv\Scripts\activate

# Activate (macOS/Linux)
source venv/bin/activate

# Install packages
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```

See [00_getting_started/00_installation_guide.md](00_getting_started/00_installation_guide.md) for detailed setup instructions and troubleshooting.

---

## How to Use This Repository

### Learning Path

1. **Start from Module 0** if you're new to Python or Jupyter
2. **Work through notebooks sequentially** within each module - concepts build on each other
3. **Run all code cells** yourself - typing code improves retention
4. **Complete the exercises** in each notebook before checking the solutions

### Notebook Structure

Each learning notebook follows a consistent format:

1. **Learning Objectives** - What you'll learn
2. **Concepts** - Explanations with runnable examples
3. **Exercises** - Practice problems (3-5 per notebook)
4. **Solutions** - Collapsed/hidden solutions (click to reveal)
5. **Summary** - Key takeaways and next steps

### Comprehensive Tests

Each module (1-8) includes a comprehensive test to assess your understanding:

| File | Description |
|------|-------------|
| `test.ipynb` | Test questions **without solutions** - complete this to test yourself |
| `test_solutions.ipynb` | The same test **with complete solutions** - review after attempting |

**Recommended workflow:**
1. Complete all notebooks in a module
2. Open `test.ipynb` and attempt all questions without referring to the lessons
3. Check your answers against `test_solutions.ipynb`
4. Review any topics where you struggled before moving to the next module

### Capstone Projects

Module 99 contains six capstone projects that integrate skills from multiple modules:

1. **Data Analysis Project** - End-to-end analysis with Pandas and Matplotlib
2. **Scientific Computing Project** - Numerical simulation with NumPy and SciPy
3. **Cloud Data Pipeline** - AWS integration with Boto3
4. **Django Web Application** - Complete CRUD app with models, views, templates, forms
5. **Database Analytics Dashboard** - SQL + Pandas + Matplotlib visualization
6. **Full-Stack Data Application** - Django + SQL + Pandas + Matplotlib integrated

---

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

### Module 7: SQL in Python
1. SQLite Basics - Connecting, creating databases and tables
2. CRUD Operations - INSERT, SELECT, UPDATE, DELETE
3. Queries and Joins - WHERE, ORDER BY, GROUP BY, JOINs
4. Pandas SQL Integration - read_sql, to_sql, combined workflows

### Module 8: Django
1. Django Introduction - Projects, apps, settings, and structure
2. Models and ORM - Defining models, migrations, QuerySets
3. Views and URLs - Function/class-based views, URL routing
4. Templates - Django Template Language, inheritance, static files
5. Forms and Admin - Form handling, ModelForms, admin customization

### Module 99: Capstone Projects
1. Data Analysis Project - Pandas, Matplotlib
2. Scientific Computing Project - NumPy, SciPy
3. Cloud Data Pipeline - Boto3, AWS
4. Django Web Application - Django full CRUD
5. Database Analytics Dashboard - SQL, Pandas, Matplotlib
6. Full-Stack Data Application - Django, SQL, Pandas, Matplotlib

---

## Directory Structure

```
cloudtraining-python/
├── README.md
├── requirements.txt
├── .devcontainer/
│   └── devcontainer.json          # GitHub Codespaces configuration
├── 00_getting_started/
│   ├── 00_installation_guide.md
│   └── 01_jupyter_basics.ipynb
├── 01_python_fundamentals/
│   ├── 01_variables_and_types.ipynb
│   ├── ... (10 learning notebooks)
│   ├── test.ipynb                 # Module test (no solutions)
│   └── test_solutions.ipynb       # Module test (with solutions)
├── 02_numpy/
│   ├── ... (5 learning notebooks)
│   ├── test.ipynb
│   └── test_solutions.ipynb
├── 03_matplotlib/
│   ├── ... (4 learning notebooks)
│   ├── test.ipynb
│   └── test_solutions.ipynb
├── 04_pandas/
│   ├── ... (6 learning notebooks)
│   ├── test.ipynb
│   └── test_solutions.ipynb
├── 05_scipy/
│   ├── ... (4 learning notebooks)
│   ├── test.ipynb
│   └── test_solutions.ipynb
├── 06_boto3/
│   ├── ... (4 learning notebooks)
│   ├── test.ipynb
│   └── test_solutions.ipynb
├── 07_sql/
│   ├── 01_sqlite_basics.ipynb
│   ├── 02_crud_operations.ipynb
│   ├── 03_queries_and_joins.ipynb
│   ├── 04_pandas_sql_integration.ipynb
│   ├── test.ipynb
│   └── test_solutions.ipynb
├── 08_django/
│   ├── 01_django_introduction.ipynb
│   ├── 02_models_and_orm.ipynb
│   ├── 03_views_and_urls.ipynb
│   ├── 04_templates.ipynb
│   ├── 05_forms_and_admin.ipynb
│   ├── test.ipynb
│   └── test_solutions.ipynb
├── 99_capstone/
│   ├── 01_data_analysis_project.ipynb
│   ├── 02_scientific_computing_project.ipynb
│   ├── 03_cloud_data_pipeline.ipynb
│   ├── 04_django_web_application.ipynb
│   ├── 05_database_analytics_dashboard.ipynb
│   └── 06_fullstack_data_application.ipynb
└── data/
    └── (reserved for datasets - samples currently created inline)
```

---

## License

This course material is provided for educational purposes.
