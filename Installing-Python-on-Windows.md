# Tutorial: Installing Python on Windows


Python is a popular open-source, high-level programming language. It's intuitive and offers many helpful tools and libraries — Python is a powerful data science asset to have in your toolkit. To start working with Python, we first need to download it and install it on our operating system (in this case, Windows).

---

## How to Install Python on Windows

There are two main ways to install Python on Windows:  
1. Installation from the official [Python website](https://www.python.org/).  
2. Installation using [Anaconda](https://www.anaconda.com/), a convenient distribution of Python and R programming languages.

- **Choose the official Python installation** if you're a programmer working on web development, network programming, or general-purpose software applications.
- **Choose Anaconda** if you're focused on data science and machine learning. Anaconda provides:
  - 1500+ built-in Python and R data science packages.
  - Popular Python IDEs like Jupyter Notebook.
  - A graphical user interface (GUI) for ease of use.

---

## Step 1: Check if Python is Already Installed

Before installing Python, check if it’s already installed on your computer.

1. Open Command Prompt (search `cmd` in Windows Search) or Windows PowerShell (right-click the `Start` button and select `Windows PowerShell`).
2. Type:
   ```sh
   python -V
   ```
   This command shows the installed Python version (if any).
3. To check the installation path, type:
   ```sh
   where.exe python
   ```

---

## Step 2: Install Python from the Official Website

If Python isn’t installed, follow these steps to download and install it from the official Python website.

---

### **Download Python**

1. Open the [Python Releases for Windows](https://www.python.org/downloads/windows/) page.
2. Select your desired Python version.
3. Download the Python executable installer.

![Python Releases for Windows](https://www.dataquest.io/wp-content/uploads/2022/01/python-releases-for-windows.webp)

---

### **Decide Between Python 2 and Python 3**

- **Python 3** (released in 2008):
  - Simpler syntax.
  - Extensive libraries, especially for data science.
  - Actively supported by the Python community.

- **Python 2** (no longer supported):
  - May be required for legacy projects or older scripts.

For new projects, Python 3 is recommended. If you need Python 2, download the `Windows x86-64 MSI installer` to match your Windows architecture.

![Python Files](https://www.dataquest.io/wp-content/uploads/2022/01/python-files-img1-1024x343.webp)

To download Python 3, choose the appropriate installer for your Windows version:

![Python Files](https://www.dataquest.io/wp-content/uploads/2022/01/python-files-img2-1024x340.webp)

---

### **Install Python 2**

1. Run the downloaded Python 2 installer.
2. Select the default options during installation.

![Python Installer](https://www.dataquest.io/wp-content/uploads/2022/01/python-installer-img1.webp)

---

### **Install Python 3**

1. Run the Python 3 installer.
2. On the first screen:
   - Check "Add Python to PATH."
   - Click "Install Now."

![Python Installer](https://www.dataquest.io/wp-content/uploads/2022/01/python-installer-img4.webp)

3. After installation, select "Disable Path Length Limit."

![Python Installer](https://www.dataquest.io/wp-content/uploads/2022/01/python-installer-img5.webp)

---

## Step 3: Verify Python Installation

1. Open Command Prompt.
2. Type:
   ```sh
   python -V
   ```
   If both Python 2 and Python 3 are installed, Python 2 may take priority. To check Python 3, type:
   ```sh
   python3 -V
   ```

---

## Step 4: Install Python Using Anaconda Navigator

For data science or machine learning, installing Python through [Anaconda Navigator](https://www.anaconda.com/) is recommended.

1. Open the [Anaconda Individual Edition](https://www.anaconda.com/) page.
2. Download the Windows installer.

![Install Python from Anaconda](https://www.dataquest.io/wp-content/uploads/2022/01/install-python-from-anaconda-1024x608.webp)

3. Run the installer and follow the default options.

![Run the Installer](https://www.dataquest.io/wp-content/uploads/2022/01/anaconda-run-the-installer.webp)

---

## Step 5: Run Python

### **Using the Official Installation**

1. Search for `IDLE` in Windows Search.
2. Open the desired version of IDLE.
3. Start coding in Python.

![IDLE Shell](https://www.dataquest.io/wp-content/uploads/2022/01/idle-shell-1-1024x203.png)

---

### **Using Anaconda**

1. Open `Anaconda Navigator`.
2. Select an application, like Jupyter Notebook.
3. Create and run a new Python notebook.

![Jupyter Notebook](https://www.dataquest.io/wp-content/uploads/2022/01/anaconda-navigator-jupyter-notebook-1024x545.png)

---

## Step 6: Update Python

### **From the Official Website**

Visit the [Python Releases for Windows](https://www.python.org/downloads/windows/) page, download the latest version, and run the installer.

![Upgrade Python](https://www.dataquest.io/wp-content/uploads/2022/01/upgrade-python1.png)

---

### **Using Anaconda**

1. Open `Anaconda Prompt`.
2. Type:
   ```sh
   conda update python
   ```

To create a new virtual environment with the latest Python version:
```sh
conda create -n python_latest python=3.10
conda activate python_latest
```

![Anaconda Prompt](https://www.dataquest.io/wp-content/uploads/2022/01/anaconda-prompt3.png)

---

## Conclusion

In this tutorial, we covered:

1. Checking for Python installations.
2. Installing Python from the official website or using Anaconda.
3. Running Python scripts on Windows.
4. Updating Python to the latest version.

Now, you’re ready to start coding in Python!
