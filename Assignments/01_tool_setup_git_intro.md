# Assignment 01: Setup Course Tools & Git Introduction

## Getting Setup
1. Create an account on GitHub (https://github.com).  An understandable and
professional user name is suggested.  
   

2. To communicate your GitHub user name to us, you will open a GitHub issue 
with that information.
   1. Go into the BME547 repository (<https://github.com/dward2/BME547>) and 
  click on "Issues" in the tab bar at the top of the page.
   2. Click on the green "New issue" button.
   3. In the title, enter your name and the GitHub user name you created. For 
  example, "David Ward - dward2".
   4. In the comment area, please include your Duke e-mail address and whether
  your primary computer for this class is running Windows, macOS, or Linux.
   5. Click the green "Submit new issue" button.
 
 
3. Download and install `git` at https://git-scm.com.  We will be using 
`Git Bash`, *not* a GUI client.
   + **MAC** users:   
     `git` is likely already installed.  Open a Terminal window
and type `git --version`.  If you see a version number, it is already
installed.  If not, you will need to download it from the site above.
   + **Windows** users have two options:
     1. install from the above website (recommended) which will install the
   GitBash command window (see <a href="../Resources/installations.md">
   installations</a> for additional details), or
     2. use the Windows Subsystem for Linux 
    ([Ubuntu Linux Subsystem (Windows 10)](https://docs.microsoft.com/en-us/windows/wsl/about)) 
    with Ubuntu allowing you to access `git` through Linux.  
    Note - this second option does not install `git` in your Windows environment, 
    so other Windows applications that have `git` hooks will not work.
   + **Everyone**: Add your name and e-mail to your local Git configuration by following the
     instructions under **Config**  on [this page](/Resources/Git/GitCommands.md#config). 


4. Set up an SSH key to allow local authentication with GitHub:
   1. Visit <https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh>
   2. From the page above, follow the instructions under the links:
      * [Generating a new SSH key and adding it to the ssh-agent](https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
      * [Adding a new SSH key to your GitHub account](https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account)
      * [Testing your SSH connection](https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/testing-your-ssh-connection)
   3. To automatically load your SSH keys when starting git, follow the 
    instructions at [Working with SSH key passphrases](https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/working-with-ssh-key-passphrases)


5. Download and install `python` at https://www.python.org/. (As of 
   August 17, 2021, the latest version is 3.9.6.)
   + **Mac** users:  
     * Python is likely already installed.  Open a Terminal window 
       and enter `python --version`.  You should see something like `Python 3.7.0`.
     * If the version number is 3.6 or higher, you are good to go.
     * If the version number is 2.7, enter `python3 --version` into the terminal 
       window and see if version 3 is also installed.  If not, you will need to 
       install `python3`.
   Do not try to delete or "upgrade" the 2.7 version currently on your 
   computer as it is a part of the macOS installation.
     * If python does not start at all, you will need to install `python3`.    
   Info on installing `python3` on macOS can be found at:      
       * <https://docs.python.org/3/using/mac.html>
       * <http://osxdaily.com/2018/06/13/how-install-update-python-3x-mac/>
       * <https://opensource.com/article/19/5/python-3-default-mac> _(if you are
     comfortable with using more advanced virtual environment options for
     managing your python versions)_.
     * Note that if you have both `python2` and `python3` installed on your 
     computer, it is possible that you will have to enter `python3` in place
     of `python` to run the correct version.  Alternatively, you can set up an
     alias by either:
       + entering `echo "alias python=/usr/local/bin/python3.7" >> ~/.bashrc` (`echo "alias python=/usr/local/bin/python3" >> ~/.zshrc` for macOS 10.15 or later)
       at the terminal prompt, or
       + manually editing the `.bashrc` (`.zshrc` for macOS 10.15 or later) file to include the line 
       `alias python=/usr/local/bin/python3.8`.  Note that you need to make
       sure that the path (`/usr/local/bin/python3.8`) matches the actual
       path on your computer.  For example, verify the version number is
       correct.
       + You will need to do the same thing with the `pip` package installer.
       Type `pip --version` at the command line and an output similar to
       `pip 19.0.3 from /Library/Python/2.7/site-packages/pip-19.0.3-py2.7.egg/pip (python 2.7)`
       will be shown.  If it refers to version 2, type `pip3 --version` to
       make sure that `pip3` was installed as part of the  `python3` install
       (it should have been).  Then, if you like, you can alias the `pip3` via
       `echo "alias pip=/usr/local/bin/pip3" >> ~/.bashrc`, (`echo "alias python=/usr/local/bin/pip3" >> ~/.zshrc` for macOS 10.15 or later), or whatever the
       correct path should be.
    
   + **Windows** users have three options:  
     1. Download and install from <https://www.python.org/> as described above.
   Follow additional guidelines found [here](../Resources/installations.md) for
   installation.
     2. Install Anaconda Python from 
   https://www.anaconda.com/download.  You can download the complete 
   Anaconda package or Miniconda which brings in the bare minimum of packages 
   and then install what is necessary in virtual environments, but each project 
   will require more download overhead.
     3. Installing and using the [Ubuntu Linux Subsystem (Windows 10)](https://docs.microsoft.com/en-us/windows/wsl/about), 
   and running `python` from within that environment.  This approach will give 
   you a legitimate Linux environment, but there is overhead to running GUI 
   applications through an X-server, which adds more complexity and can be 
   slower for complex interfaces.


6. You will want a code writing environment / text editor that makes life 
easier for you as your projects get more complex.  Options include:
   + Terminal Editors
      + [VIM](http://www.vim.org)
      + [nano](https://www.nano-editor.org/)
   + Code / Text editors
      + [GitHub Atom](https://atom.io/)
      + [Visual Studio Code](https://code.visualstudio.com/)
      + [Sublime Text](https://www.sublimetext.com/)
      + [Notepad++](https://notepad-plus-plus.org/)
        (See [Resources/Notepad++.md](../Resources/notepad++.md) for set-up
        info and markdown plug-ins)
   + Browser-based Interactive
     + [Jupyter Lab](https://jupyterlab.readthedocs.io/en/latest/#)
   + Full-featured IDE (integrated development environment)
     + [PyCharm](https://github.com/dward2/BME547/tree/master/Resources/PyCharm) 
    (professional edition free to use in academic setting, also includes
    Python interpreter).
     + [Spyder](https://www.spyder-ide.org/) (free IDE included with Anaconda)
    
    Check to see if your chosen text editor has the ability (or an extension) to
    edit and render Markdown text.  If so, set that up. 

## Checking Set-up
A GitHub repository has been created with some simple steps for you to follow
to verify that can execute git and Python on your computer.  Please visit
<https://github.com/dward2/setup_verification> and follow the instructions
found there.

## Learning Git
If you really can't wait to get started...
1. Never used git before?  Start with these resources:  
  https://try.github.io/  
  https://www.codecademy.com/learn/learn-git  
  https://www.git-tower.com/learn/cheat-sheets/vcs-workflow  
  http://gitimmersion.com/  
  https://www.atlassian.com/git/tutorials/setting-up-a-repository

1. Familiar with git (or just completed the exercises above)?  Give this a try:
  http://learngitbranching.js.org/

1. Having trouble?  We'll be covering usage of many of these tools in upcoming
  lectures.  

## What We Will Eventually Learn How To Do In Git:
  + Create a git repository on your local computer.
  + Create a local file, then add and commit it to your local repository.
  + Edit your local file, adding and committing those edits.
  + Create a remote repository on GitHub that has the same name as your local repository.
  + Add the remote repository (origin) URL to your local repository.
  + Push your local repository to GitHub.
  + Create a local branch, create/add/commit a new file.
  + Push new local branch to GitHub.
  + Merge new branch on GitHub into main branch on GitHub.
  + Pull the updated main branch into local repository.
