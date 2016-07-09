# Dev Setup

## Sublime Text 3

Install (SublimeText3)[https://www.sublimetext.com/3] Portable Version for Windows (likely 64-bit).

Unzip the file into a folder where you want to house your ST3 installation

Open the folder and run `sublime_text.exe`.

Go to (PackageControl.io)[https://packagecontrol.io/installation], copy the code for Sublime Text 3. Go back to ST3 Editor and go to `View -> Show Console`. Paste the code into the console window and hit enter.

Restart Sublime (Close and Reopen)

### SublimeText3 Themes

Run `ctrl+shift+p` to open the ST3 prompt and type `install package` to open the `Package Control: Install Package` window. Search for `Material Theme` and hit `enter` to install. The message that pops up lists some recommended preferences for a better experience. Go ahead and copy those settings and open `Preferences -> Settings - User` and paste them in. Save the file `ctrl+s` and close it.

Run `ctrl+shift+p` again and install `Sidebar Enhancements` and potentially `Material Theme Sidebar` or anything else you want for themes.

### Python

(Install Python)[https://www.python.org/downloads/windows/] by downloading and running, choose to install in your `C:/Users/<yourusername>/Python35` folder. Click through the menus to install. You need to ensure `python.exe` and `pip.exe` is in your path variable. Start menu `edit environment variable` search for your own account should work. Here is (a guide of some sort)[http://johnatten.com/2014/12/07/adding-and-editing-path-environment-variables-in-windows/] the menu is the same but you are doing the non-admin version. Should be adding the path variable as `C:/users/<yourusername>/Python35;C:/users/<yourusername>/Python35/bin;` because you want the containing folders for `pip.exe` and `python.exe` to be in your path variable. From the command prompt `echo %PATH%` should tell you what is currently in it.

### SublimeText3 Linter

First install ST3 Linter from `package control` by typing `ctrl+shift+p` and `install package` + `enter` and search for `sublimelinter` and install it. The official docs for it are (here)[http://sublimelinter.readthedocs.io/en/latest/installation.html]

Then you need to install cpplint. Open up your terminal and run `pip install cpplint` which will install the cpplint program through python's package manager. You also (can install it from here potentially)[http://cppcheck.sourceforge.net/]. After it is installed you also need to ensure that this it is in your path variable so that if you were to type `cppcheck` in your DOS cmd prompt it would find and run the `cppcheck.exe`, you will know because you will get some output message from `cppcheck`.

Afterwards we are following the (instructions)[https://github.com/SublimeLinter/SublimeLinter-cppcheck] for install SublimeLinter-cppcheck. We can use `ctrl+shift+p` then `install package` + `enter` and search for `sublimelinter-cppcheck` and install it. Restart `ST3.exe` and it should be working, though you might need to fiddle with the (linter settings)[http://sublimelinter.readthedocs.org/en/latest/linter_settings.html]




