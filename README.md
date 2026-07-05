this is a great way to troll ur freinds if they alr know the link
## How to Convert this Script into a .exe File

You can turn this script into a standalone Windows executable using `pyinstaller`. This allows you to run it on any Windows machine without needing Python installed.

### Prerequisites
Make sure you have an icon file ready in the same folder as your script (e.g., `app_icon.ico`). You can convert any PNG or JPG to a `.ico` format using online converters.

### 1. Install PyInstaller
Open your terminal or command prompt and run:
```bash
pip install pyinstaller
```

### 2. Compile the Script with an Icon
Navigate to the folder containing your script and your icon file, then run:
```bash
pyinstaller --onefile --noconsole --icon=app_icon.ico open_link.py
```
*(Note: Replace `app_icon.ico` with the exact name of your icon file!)*

### What do these flags mean?
* `--onefile`: Bundles everything into a single, clean `.exe` file.
* `--noconsole`: Hides the black terminal/command prompt window when the script runs. The browser window will just open up out of nowhere.
* `--icon=...`: Applies your custom icon to the executable file instead of the default Windows blank icon.

### 3. Find your Executable
Once the process finishes, look inside your project folder. You will see a new folder named **`dist`**. Inside that folder, you will find your compiled **`.exe`** file, disguised and ready to deploy!
