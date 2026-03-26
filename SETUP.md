# Setup & Installation Guide

Complete guide to set up the Zomata Data Analysis project on your local machine.

## Prerequisites

- **Python 3.7+** (Python 3.9 or 3.10 recommended)
- **pip** or **conda** package manager
- **Git** for version control
- ~100 MB disk space

## Installation

### Option 1: Quick Setup with pip

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/zomata-data-analysis.git
cd zomata-data-analysis

# 2. Create a virtual environment (recommended)
python -m venv venv

# 3. Activate the virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

# 4. Install dependencies
pip install -r requirements.txt

# 5. Launch Jupyter
jupyter notebook "Zomata Data Analysis.ipynb"
```

### Option 2: Setup with Conda

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/zomata-data-analysis.git
cd zomata-data-analysis

# 2. Create conda environment
conda create -n zomata python=3.10

# 3. Activate environment
conda activate zomata

# 4. Install from requirements
pip install -r requirements.txt

# 5. Launch Jupyter
jupyter notebook "Zomata Data Analysis.ipynb"
```

## Troubleshooting

### Issue: "Python not found"
**Solution:** Ensure Python is installed and added to PATH
```bash
python --version  # Should show 3.7+
```

### Issue: "ModuleNotFoundError: No module named 'pandas'"
**Solution:** Reinstall dependencies
```bash
pip install --upgrade -r requirements.txt
```

### Issue: "Jupyter command not found"
**Solution:** Install Jupyter explicitly
```bash
pip install jupyter --upgrade
```

### Issue: Notebook kernel fails to start
**Solution:** Restart the kernel or create a new one
```bash
# In Jupyter: Kernel > Restart & Clear Output
# Or reinstall ipykernel:
pip install --upgrade ipykernel
```

## Verify Installation

Run this in a terminal to verify everything is installed:

```bash
python -c "import pandas, numpy, matplotlib, seaborn; print('✓ All packages installed successfully!')"
```

## Running the Analysis

1. Open the notebook file in Jupyter
2. Run cells sequentially (Cell > Run All, or Shift+Enter)
3. View generated visualizations and outputs
4. Review markdown cells for analysis explanations

## Project Structure

```
zomata-data-analysis/
├── Zomata Data Analysis.ipynb    # Main analysis notebook
├── Zomato data .csv              # Dataset (151 restaurants)
├── README.md                      # Project overview & insights
├── requirements.txt               # Python dependencies
├── data_dictionary.md             # Dataset schema
├── SETUP.md                       # This file
├── CHANGELOG.md                   # Version history
├── CONTRIBUTING.md                # Contribution guidelines
├── LICENSE                        # MIT License
├── .gitignore                     # Git ignore rules
└── charts/                        # Visualization outputs
    ├── Type of Restaurant.png
    ├── 2.png through 9.png
    └── ...
```

## Useful Commands

```bash
# Update dependencies later
pip install --upgrade -r requirements.txt

# List installed packages
pip list

# Deactivate virtual environment
deactivate

# Remove virtual environment (if needed)
rm -r venv  # macOS/Linux
rmdir /s venv  # Windows
```

## Next Steps

1. Read [README.md](README.md) for project overview
2. Check [data_dictionary.md](data_dictionary.md) for dataset details
3. Run the notebook to explore the analysis
4. Review [CONTRIBUTING.md](CONTRIBUTING.md) if you'd like to contribute

## Support

For issues or questions:
1. Check this guide's Troubleshooting section
2. Review [README.md](README.md) FAQ section
3. Open an Issue on GitHub with details

---

Happy analyzing! 📊
