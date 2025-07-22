# ITBA Python Package Setup Guide

Welcome to the ITBA-KIT Modeling and Simulation course! 

Big shoutout to Dr. Sebastian D'Hers, creator of this course, for providing most of the material in this repository. 

This guide will help you set up a Python development environment for this repository (folder `resources`) using **Miniconda** and **conda** virtual environments. Follow the steps below to ensure a smooth installation and reproducible workflow.

---

### 1. Install Miniconda

Miniconda is a minimal installer for conda. Download and install Miniconda for your operating system by following the official instructions:

👉 [Miniconda Installation Guide](https://www.anaconda.com/docs/getting-started/miniconda/install)

---

### 2. Learn to Manage Conda Virtual Environments

If you are new to conda environments, check out this tutorial for creating and managing environments:

👉 [How to Create Virtual Environments with Conda](https://numdifftools.readthedocs.io/en/latest/how-to/create_virtual_env_with_conda.html)

---

### 3. Create Your Environment from `itba_env.yml`

If you have the `itba_env.yml` file in this repository, you can create the environment with all required dependencies in one step:

```bash
conda env create -f itba_env.yml
```

### 4. Alternatively: Create a New Environment Manually
If you prefer to create the environment manually, run:

```bash
conda create -n itba_env python=3.12
```

### 5. Activate the Environment and Check Python Version

```bash
conda activate itba_env
python --version
```

### 6. Install Basic Scientific Libraries
Install the core libraries needed for scientific computing:

```bash
conda install -c conda-forge numpy scipy pandas matplotlib sympy cython
```

### 7. Install Spyder (Optional, but Recommended) and Sypder Notebook (to read .ipynb files)
Spyder is a powerful IDE for scientific Python development. Other alternatives are PyCharm or VS Code, for students with experience in programming.

To install Spyder:

```bash
conda install -c conda-forge spyder=6.0.7
conda install spyder-notebook -c conda-forge
```

### You're Ready!
You now have a fully functional Python environment for this course.
Happy coding!
