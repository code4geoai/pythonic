---
jupyter:
  jupytext:
    formats: ipynb,md
    text_representation:
      extension: .md
      format_name: markdown
      format_version: '1.3'
      jupytext_version: 1.16.7
  kernelspec:
    display_name: Python 3 (ipykernel)
    language: python
    name: python3
---

# Installation & Setup Guide


This installation and Setup guide will help begineers to install python , setup the environiment and start coding in a convenient way. Let's gets started.


## Option 1:
### Install Python from Official Website
1. Visit python.org.
2. Download the latest version for your OS (Windows/macOS/Linux).
3. Run the installer:
4. Check "Add Python to PATH" (Windows).
5. Verify installation: open termminal and enter.

```python
print("Hello, Python!")  
```

## Option 2:
### Anaconda or Miniconda

1. These are Package manager for Python/R.
2. It has Pre-installed data science libraries (NumPy, Pandas, etc.).

### Installation:
1. Download Anaconda or Miniconda.
2. Run the installer.
3. Verify:

```python
conda --version
```

### Creating conda (virtual environiment)
The virtual environiment are created to have Isolate project dependencies and you can avoid packages incompatibility issues.

```python
conda create --name myenv python=3.10  
conda activate myenv  
```

### IDEs for Python
if you have created your virtual environiment with conda its time to install packages.  


```python
conda install pip # pip is a package manner if not already installed.
```

### Jupyter Lab
 Install jupyter lab with command pip install jupyter lab

```python
pip install jupyter lab
```

### Launch jupyter Lab

```python
jupyter lab
```

### Jupyter Notebook
Install jupyter notebook with command pip install jupyter notebook

```python
pip install jupyter notebook
```

### Launch the Jupyter Notebook

```python
jupyter notebook
```

### VS Code

1. Download [VS Code](https://code.visualstudio.com/).
2. Install the Python Extension.
3. Install the jupyter Extension.
3. Open a new file and start coding!


### Google Colab
1. No installation needed.
2. Visit [colab.research.google.com](https://colab.research.google.com/).
3. Write code directly in the browser.
