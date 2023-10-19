### Upgrading Python to Version 3.11
Validate your Python version by typing:
```
python -V
```
If you see Python v2, then type as you may have both versions installed:
```
python3 -V
```
If you have both Python versions installed, and your python3 version is 3.11, then you can use "python3" instead of "python" to complete the lab.

### Caution Mac Users
Mac installs a system version of Python in /usr/bin/python.  **DO NOT DELETE** /usr/bin/python as it will cause your system to malfunction.

### Where is Python installed
By typing the following command, you can view the location of Python on your computer.
```
which python
```
### Old Versions of Anaconda
Many people have old versions of Anaconda installed.  IBM employees should not be using the full Anaconda installation due to enterprise licensing concerns.  Instead, you should install Miniconda.  However before you do that, delete the installations of Anaconda.  The fastest way to achieve this is:

1. Delete Anaconda and Anaconda Navigator from your Applications folder.
2. Run "which python" again to see if any other installations remain.
   - **DO NOT DELETE** /usr/bin/python as it will cause your system to malfunction.
3. Delete other versions of python using "rm -rf".  **Be very careful** when running this command is it permanently delete all folders/files in a folder.
```
rm -rf <full path to python to remove>
```

### Cleaning up your .bash_profile
When you open a Terminal window on Mac, your Bash script file located at "~/.bash_profile" is executed.  To fully remove Anaconda and other references to other Python version on your computer, you will need to remove their references from "~/.bash_profile".

To find your base home directory, run these two commands one-at-a-time:
```
cd ~
pwd
```
Your .bash_profile is located in this directory.  This is a text file so open in any text editor.  Files begining with a period are considered Hidden so you may need to unhide the file in order to open from Finder.  Learn how to [view these hidden files on a Mac](https://www.macworld.com/article/671158/how-to-show-hidden-files-on-a-mac.html).

Be careful editing if you're unfamiliar with shell scripts.  Ask a colleague or friend for help.  We're all here to help each other.   


### Miniconda Installation
[Miniconda](https://conda.io/miniconda.html) is a lighweight version of Anaconda.  The full Anaconda installation has enterprise licensing requirements that preclude using it for free as an IBMer. Please install Miniconda instead.  You may want to read [learn more about Conda Environments](https://whiteboxml.com/blog/the-definitive-guide-to-python-virtual-environments-with-conda) before proceeding.

If Conda is your choice for a Python Environment Manager, then [install miniconda](https://docs.conda.io/en/latest/miniconda.html) as the remainder of this section assumes you have it installed.

#### Upgrading Python using Miniconda
You can now upgrade the base Python version used by Miniconda by typing:
```
conda install python=3.11.3
```

### Python Base Installation
To install the latest version of Python in your base system, you can run. 
```
brew install python
```
This command will download and install the most recent Python version.

