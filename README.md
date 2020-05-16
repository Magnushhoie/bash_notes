# bash_search

BASH note-taking system directly in the terminal. Collection of collected and edited scripts I have been actively every day for the past couple of years.

### Example of use:

https://terminalizer.com/view/ef4b2b193819

Installation of dependencies:
```bash
bash setup.sh
```

Installation is relatively fast on macOS, and relatively slow if using linuxbrew on another UNIX system.

#### 1. bash_notes.sh:
Bash note-taking system with easy search and editing in place, directly from the terminal using vim.
Uses a combination of grep and vim to search references.txt or any file in ~/_References folder.

Commands:
- ref keywords: Search for keywords in references.txt
- refv keywords: Search references.txt and open at line in Vim. 
- refv filename.txt: Create new note file

### 3. setup.sh:
- Sets up references directory and adds script to .bash_profile

### 4. optional files
- Suggested vim configuration files and plugins. Installer will ask whether to install first.

