# GIT SETUP & CONFIGURATION

## 1. Identify how to install GIT
    - Download [GIT](https://git-scm.com/downloads) from git website as per your operating system.
## 2. Set initial configuration variables
    
    Step 1: Set your user name and email
    - $git config --global user.name "your name"
    - $git config --global user.email youremail@example.com
    - Important as these will be included with every commit.
    
    Step 2: Set your default text editor
    - $ git config --global core.editor emacs
    - $ git config --global core.editor "C:\Program Files (x86)\Notepad++\notepad++.exe —multiInst nosession"
    - $ git config --global core.editor "code --wait" [Visual Studio Code]
    
## 3. Introduce GIT Configuration Tool
    - Two categories of configurations
    - Client-side
      - Configuring you personal workspace preferences
      - Majority of the options available
    - Server-side
      - Configuration workflow options
      - Secure repository data
## 4. Identify the three GIT configuration levels
    - System level
      * Applies to every user on the system and all of their repositories
      * Stored in /etc/gitconfig or C:\ProgramData\git\config
      * $ git config --system
    - User level
      - Applies to all projects for the current user.
      - Stored in ~./gitconfig for C:\Users\$USER\.gitconfig
      - $ git config --global
    - Repository level
      - Applies only to the current project
      - Stored in .git/config
      - $ git config or git config --local
    - Order of Precedence
      - System < User < Repository
      
## Retrieving Configuration Settings
- --list
  - Returns all keys and values in supplied configuration
  - $git config --global --list
  - Add --show-origin option to see the origin of each key
- --get
  - Returns the value of the specified key
  - $ git config --get user.name
- --get-all
  - Returns all values for the specified key
  - $ git config --get-all user.name
