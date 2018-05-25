# FSU-Cybersecurity-Modules

| Table of Contents |
|-------------------|
|[Background](#background)|
|[Install](#install-tips)|
|[Usage](#usage)|
|[TODO](#todo)|   

## Background

This repository contains two different types of resources for practicing cybersecurity. It is part of a larger set that can be found at  [CNAP Focus Area: Integration of Hands-on Learning Experiences into Cybersecurity Curriculum](http://www.sait.fsu.edu/dod/dod.shtml)


Components include:
  -SQL Injection Module
  
  -VirtualBox importable machines with pre-installed tools.
## Virtual Machines

# this remainder of this page is under construction. 
### Ubuntu
  
### Windows 7

 

**1. Windows 7 64 bit Virtual Machine?**
- Yes: Cool you are in the same place as us.
- No: AngryIDA has not been tested on other operating systems and may have unintended results. 

**2. IDA Pro 6.9?**
- Yes: Install Microsoft Visual C++ 2015 or newer and update the .NET Framework.
- No: Install IDA 6.9 then return here.

**3. IDA Python Plug-In Working?**
- Yes: Continue to the next step.
- No: Currently no tips to solve this problem.

**4. Python 2.7 is installed?**
- Yes: Keep going.
- No: There are many resources online for installing python 2.7 on virtually every system.

**5. Python package manager pip is installed?**
- Yes: Awesome, one step closer.
- No: Installing pip is straightforward and help can be found online.

**6. angr is installed and working?**
- Yes: Skip to the next step.
- No: Try this...
    + Install Microsoft Visual Studio 2017 (Really you just need the developer command prompt)
    + Install the Microsoft Visual C++ Compiler for Python 2.7
    + Inside the Microsoft Visual Studio Developers Command Prompt run the following commands:
        * pip install -I --pre --no-use-wheel capstone-windows
        * pip install pyvex
        * pip install unicorn
        * pip install simuvex
        * pip install angr

**7. Downloaded this repository (At least the file AngryIDA.py)?**
- Yes: You are ready to use AngryIDA!
- No: Why not?

## Usage

**1. Start IDA Pro**
- One option: Drag and drop the file you wish to analysis on the IDA Pro shortcut.

**2. Start AngryIDA**
- Alt+F7
- Navigate to AngryIDA.py file
- Select AngryIDA.py

**3. Menu**
- The AngryIDA menu is located in the context menu of IDA View-A
    + Right click inside of IDA View-A
    + Hovering over AngryIDA expands the AngryIDA menu.

**4. Exploring**
- Handling find and avoid address:
    + Right click on the desired address in IDA View-A:
        * Select Finds or Avoids from the AngryIDA menu:
            - Select Set/Remove/View 
- Remove all find and avoid address:  
    + Right click in IDA View-A:
        * Select Refresh from the AngryIDA menu
- Set up symbolic stdin:
    + Right click in IDA View-A:
        * Expand Explore from the AngryIDA menu:
            + Select options:
                - Fill in the presented options form
- Explore options:
    + Right click in IDA View-A:
        * Expand Explore from the AngryIDA menu:
            + Select options:
                - Fill in the presented options form
- Explore:
    + Right click in IDA View-A:
        * Expand Explore from the AngryIDA menu:
            + Select run

## TODO

* Documentation
* Code improvement based on Pylint code scoring.
* Hotkeys
* How to stop angr path exploration?
* Code coverage display through path highlighting. 
* Revert changes made by the application when exited. 
* Handle all forms of symbolic memory (stdin, files, arguments).
* Symbolic stdin: 
    - Handle multiple stdin streams
    - Remove created input streams

#


