# Tutorial: Installing Python on Mac

Python is one of the most powerful programming languages, widely used in data science, machine learning, and big data analytics. Installing Python is essential for all programmers. As a novice programmer, you may wonder how to install or update Python on your Mac properly. Here, we’ll walk through the different ways of installing and updating Python on macOS.

Then, to write and run our Python code in an integrated development environment (IDE), we will learn how to install and configure Visual Studio Code on Mac. There are different methods for installing and updating Python on Mac, but let’s stick to the third principle of the **Zen of Python** that says: “_Simple is better than complex._” Accordingly, we will try simple methods rather than complex ones. Before we jump into learning how to install or update Python on Mac, let’s review what we’re going to discuss in this tutorial:

- [Installing and updating Python on Mac](#installing-python-mac)
- [Installing Visual Studio Code on Mac](#installing-visual-studio-mac)
- [Running our first Python script on Mac](#running-python-script-mac)

---

## Installing and Updating Python on Mac

I have two pieces of news for you: one is good, the other bad. The good news is that for the sake of compatibility with legacy systems, Python 2.7 is pre-installed on your Mac. The bad news is that Python 2.7 has been retired. Therefore, it isn't recommended for new developments. If you want to take advantage of the new Python version with its many features and improvements, you need to install the latest Python alongside the version that comes pre-installed on macOS.

Before we start installing the latest version of Python, let’s see why there are different versions of the same programming language. All programming languages evolve by adding new features over time. The programming language developers announce these changes and improvements by increasing the version number.

---

### Install Python 3 as a Part of the Command Line Developer Tools

To check the current version of Python that is already installed, open the **Terminal** application by pressing `Command + Space`, typing **Terminal**, and hitting `Return`. Now, type the following command and hit `Return`:

```bash
python --version
```

You’ll likely see:

```bash
Python 2.7.18
```

Next, try this command to check if Python 3 is installed on your Mac:

```bash
python3 --version
```

If Python 3 isn’t installed, you may see this message:

```bash
xcode-select: note: no developer tools were found at '/Applications/Xcode.app', requesting install. Choose an option in the dialog to download the command line developer tools.
```

A dialog box will appear, stating that this command requires the **Command Line Developer Tools**. Let’s briefly explain: this package includes tools mostly used in development, such as `make`, `git`, `python3`, etc. Although there are other ways to install Python 3.x on Mac, I recommend installing the Command Line Developer Tools because it provides many additional tools for development.

To install the tools:
1. Click the **Install** button in the dialog box.
2. Follow the steps to complete the installation process.

After installation, rerun the command to confirm Python 3 installation:

```bash
python3 --version
```

You should see something like:

```bash
Python 3.8.9
```

---

### Install Python 3 with the Official Installer

Downloading the latest Python version from the official [Python website](https://www.python.org/downloads/) is another method. Here’s how:

1. Visit [python.org/downloads](https://www.python.org/downloads/). The website detects your operating system and displays a button to download the latest Python installer for macOS. If it doesn’t, click **macOS** and select the latest release.

   ![Installing Python on Mac](https://www.dataquest.io/wp-content/uploads/2022/01/installing-python-on-mac-screenshot-s-1024x578.webp)

2. Double-click the downloaded package to start the installation process. Follow the wizard to complete the installation. Usually, the default settings work well. You may need to enter your Mac password to agree to the installation.

   ![Installing Python on Mac](https://www.dataquest.io/wp-content/uploads/2022/01/installing-python-on-mac-screenshot-r-1024x778.webp)

   > **Note**: If you’re using an Apple M1 Mac, you need to install **Rosetta**. Rosetta enables Intel-based features to run on Apple silicon Macs.

3. Once the installation completes, the Python folder will open automatically.

   ![Installing Python on Mac](https://www.dataquest.io/wp-content/uploads/2022/01/installing-python-on-mac-screenshot-q-1024x561.webp)

4. Verify the installation by double-clicking **IDLE** (Python’s built-in IDE). If everything works correctly, IDLE will show the Python shell:

   ![Installing Python on Mac](https://www.dataquest.io/wp-content/uploads/2022/01/installing-python-on-mac-screenshot-p-1024x728.webp)

5. Write and run a simple Python program in IDLE. Type the following code:

   ```python
   print("Hello, World!")
   ```

---

## Installing Visual Studio Code on Mac

Although we can use **IDLE** or the terminal for writing Python scripts, a powerful, extensible, and lightweight code editor like **Visual Studio Code (VS Code)** is preferred.

1. Download VS Code for macOS from the [official website](https://code.visualstudio.com/).

   ![Installing Visual Studio Code on Mac](https://www.dataquest.io/wp-content/uploads/2022/01/installing-python-on-mac-screenshot-m-1024x574.webp)

2. Double-click the downloaded file to extract its contents.

   ![Installing Visual Studio Code on Mac](https://www.dataquest.io/wp-content/uploads/2022/01/installing-python-on-mac-screenshot-l-1024x687.webp)

3. Move the extracted **Visual Studio Code** application to the **Applications** folder.

   ![Installing Visual Studio Code on Mac](https://www.dataquest.io/wp-content/uploads/2022/01/installing-python-on-mac-screenshot-k-1024x687.webp)

4. Launch VS Code and open a folder where your Python scripts will reside. For example, create a new folder on your **Desktop**, name it `py_scripts`, and open it in VS Code.

   ![Installing Visual Studio Code on Mac](https://www.dataquest.io/wp-content/uploads/2022/01/installing-python-on-mac-screenshot-j.webp)

5. Create a new file with a `.py` extension (e.g., `prog_01.py`). VS Code will detect the `.py` extension and prompt you to install the Python extension.

   ![Installing Visual Studio Code on Mac](https://www.dataquest.io/wp-content/uploads/2022/01/installing-python-on-mac-screenshot-h-1024x710.webp)

6. Install the Python extension by clicking the **Install** button.

   ![Installing Visual Studio Code on Mac](https://www.dataquest.io/wp-content/uploads/2022/01/installing-python-on-mac-screenshot-g-1024x710.webp)

7. Select the Python interpreter by clicking on the **Select Python Interpreter** button.

   ![Installing Visual Studio Code on Mac](https://www.dataquest.io/wp-content/uploads/2022/01/installing-python-on-mac-screenshot-d-1024x710.webp)

---

## Running Our First Python Script on Mac

Now that everything is set up, let’s write and run a Python script in VS Code.

1. Write the following code in the `.py` file you created:

   ```python
   print("Hello, World!")
   name = input("What's your name? ")
   print("Hello, {}!\nWelcome to Dataquest!".format(name))
   ```

2. Run the code by clicking the ▶️ button in the top-right corner of VS Code. The output will appear in the integrated terminal. First, it will display:

   ```bash
   Hello, World!
   ```

   Then it will ask for your name. Enter your name and hit `Return`. It will output:

   ```bash
   Hello <your name>!
   Welcome to Dataquest!
   ```

   ![Running Python on Mac](https://www.dataquest.io/wp-content/uploads/2022/01/installing-python-on-mac-screenshot-a-1024x729.webp)

---

## Conclusion

In this tutorial, we learned how to install and update Python on macOS, install and configure Visual Studio Code for Python development, and run our first Python script. In the next tutorial, we’ll explore [Python virtual environments](https://www.dataquest.io/blog/a-complete-guide-to-python-virtual-environments/) and how to use them. Congratulations, Pythonista!

For more learning, check out:
- [Dataquest's Introduction to Python course](https://www.dataquest.io/course/introduction-to-python/)
- [Data Analyst in Python Path](https://www.dataquest.io/path/data-analyst)
- [Data Scientist in Python Path](https://www.dataquest.io/path/data-scientist)
