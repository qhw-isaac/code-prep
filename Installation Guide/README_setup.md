# Local Environment Setup Guide

This guide will help you set up your local computer to run the materials in the MFRE Welcome Package. It includes instructions for installing Python, Anaconda, and VS Code, creating virtual environments, and running Jupyter Notebooks.

## Step 1: Install Anaconda (Python)

1. Go to the official Anaconda website: https://www.anaconda.com/download
2. Choose the version for your operating system (Windows, macOS, or Linux).
3. Download the installer (Python 3.x version).
4. Run the installer and follow the on-screen instructions. Keep the default options unless you know what you are doing.
5. After installation, open the Anaconda Navigator or Anaconda Prompt to verify it works.

To test your installation:

- Open the Anaconda Prompt or Terminal
- Type: `conda --version`

You should see the version number printed.

## Step 2: Install VS Code (Visual Studio Code)

1. Go to the official VS Code website: https://code.visualstudio.com
2. Download the installer for your operating system.
3. Run the installer and follow the instructions.
4. After installation, launch VS Code.

### Recommended Extensions

In VS Code, go to the Extensions panel and install the following:

- Python (by Microsoft)
- Jupyter (by Microsoft)
- R Extension (by R Tools or Ikuyadeu)

## Step 3: Create a Virtual Environment

It is good practice to use a virtual environment so that your Python dependencies stay organized.

1. Open Anaconda Prompt (Windows) or Terminal (macOS/Linux).
2. Run the following command to create a new environment:

   ```
   conda create -n mfre python=3.10
   ```

3. Activate the environment:

   ```
   conda activate mfre
   ```

4. Install required packages:

   ```
   conda install jupyter pandas matplotlib numpy
   ```

You can now use this environment to run all Python notebooks in the welcome package.

## Step 4: Open and Run a Jupyter Notebook

### Option 1: Using Anaconda Navigator

1. Launch Anaconda Navigator.
2. Click on the "Launch" button under Jupyter Notebook.
3. Your browser will open. Navigate to the folder where the welcome package is saved.
4. Click on any `.ipynb` file to open and run it.

### Option 2: Using Terminal or Anaconda Prompt

1. Navigate to your folder containing the notebooks. For example:

   ```
   cd Desktop/welcome_package/python
   ```

2. Start Jupyter Notebook:

   ```
   jupyter notebook
   ```

3. A browser window will open automatically. Click on any `.ipynb` file to begin.

## Step 5: Running RMarkdown Files

To run `.Rmd` files (RMarkdown):

1. Install RStudio: https://posit.co/download/rstudio-desktop
2. Open RStudio and open the `.Rmd` file.
3. Click the "Knit" button at the top to render the file.

If prompted, install missing packages.

## Additional Tips

- Always activate your environment before working:

  ```
  conda activate mfre
  ```

- To update packages:

  ```
  conda update --all
  ```

- To deactivate:

  ```
  conda deactivate
  ```

## Questions?

If you encounter any issues during setup, note them down and we will review common setup questions at the start of the boot camp.
