# Instructions for manual installation of the DB1 tools if you don’t want to use the install scripts or they fail.

## Install Visual Studio Code 

### Download
- Go to Visual Studio Code’s website.
- Click the Windows installer button.
Run the Installer:
- Once downloaded, double-click the .exe file (likely in your Downloads folder).
- Click Next on prompts, agree to the license, and choose an install location if you want to.
- When you see “Select Additional Tasks,” check any option mentioning “Add to PATH” or “Register code as an editor.” This helps VS Code run smoothly.
- Click Install, then Finish.

### Open VS Code
- After installation, you’ll find a Visual Studio Code shortcut on your Desktop or in your Start Menu.
- Double-click to launch it. 

## Install Python 3.10+ 

### Download

- Go to Python’s official downloads page.
- Under the “Latest Python 3 Release” heading (version 3.10 or higher), click Windows installer (64-bit) (or 32-bit if that’s your system).

### Run the Installer

- Double-click the downloaded .exe in your Downloads folder.
- Important: On the first screen, check “Add Python 3.x to PATH” at the bottom.
- Click Install Now.
- Once it’s done, click Close.

### Verify Installation (Optional)

- You can confirm Python is installed by typing “Python” in your Windows Start Menu search bar.
- You should see “Python 3.x” and “IDLE (Python 3.x)” among your apps. If you open IDLE, you’ll see a Python shell that shows your Python version at the top.

## Use the DB1 project from the install files 

1.	Download the install files for the DB1 tools from DTU Learn. Available as a zip file.
2.	Extract the contents of the zip file and inside you’ll find a directory called db1. This is an example project that you can use to work with the Huzzah board.

## Create a Virtual Environment in VS Code 

What’s a virtual environment?
It’s a neat trick so that any Python packages you install do not clutter or interfere with other Python projects or your system.

Open Your Folder in VS Code:
- Start VS Code (from your Start Menu or Desktop icon).
- In the top menu, choose File → Open Folder…
- Select the db1 folder you just gotten from the installation files.
Install the Python Extension:
- In VS Code, look on the left sidebar for the Extensions icon (it looks like four blocks).
- Click it, type “Python” in the search box.
- Click Install for the “Python” extension by Microsoft.
Let the Python Extension Help You Create an Environment: - Once installed, click the View menu → Command Palette… (or press Ctrl + Shift + P).
- Type Python: Create Environment and select it from the list.
- VS Code will guide you through creating a virtual environment:
Choose “Venv” or “Virtual environment” when prompted. 
If asked, pick “Python 3.10.x” (or the latest you have).
- Wait for it to finish. It may ask if you want to use this environment. Click Yes or Use this environment.
How to Confirm:
- In the bottom-right corner of VS Code, you may see something like “Python 3.10.11 (venv: venv).”
- This means your project is using the local virtual environment instead of the system-wide Python.

