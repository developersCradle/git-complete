
## Section 05 Text Editor Installation

Text Editor Installation

# What I Learned

# Text Editor Installation Overview

- We can cheese what text editor what we would want to use.

<img src="textEditorPossibilities.JPG" alt="alt" width="300"/>

# Windows Text Editor: Notepad++ Installation

- [Notepad++](https://notepad-plus-plus.org/)

- We can add to to system variables to start from cmd!

# Configure Notepad++ with Git (Windows Only)

- Create `.bash_profile` file to home directory.
    - Configure Notepad++ with Git.

### content of .bash_profile
```
alias npp='notepad++.exe -multiInst -nosession'
```
- Now command `npp` should launch Notepad++ automatically.

Adding core editor to git config.
- `git config --global core.editor "notepad++.exe -multiInst -nosession"`

<img src="gitNotepadConfiguring.JPG" alt="alt" width="300"/>

1. Setting core editor into global config. `git config --global core.editor "notepad++.exe -multiInst -nosession"`
2. Listing global configurations. `git config --global --list`

3. Testing if tool starts with default settings `git config --global -e`

# Mac Text Editor: TextMate 2 Installation

- Skipping, won't use mac

# Configure Text Mate 2 with Git (Mac Only)

- Skipping, won't use mac
