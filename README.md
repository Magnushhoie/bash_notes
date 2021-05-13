# bash_notes

Personal bash note-taking system using the terminal. Multi-line searches and edits note files using grep, less and Vim.

Daily driver for managing code snippets since 2019. See [references.txt](references.txt) for example note file.

## Installation

Sets up ~/_bash_notes directory and adds ref and refe as aliases to ~/.bash_profile. Edit [config.txt](config.txt) to change default notes directory and editor.

```bash
git clone https://github.com/Magnushhoie/bash_notes/
cd bash_notes
bash setup.sh
```

## Usage

```python
# ref.sh: Multi-line search for keywords in references.txt or other .txt files in note folder
ref # Open references.txt in less
ref <keywords> # Multi-line search for keywords, open at matches
ref notefile2 <keywords> # Search for keywords in notefile2.txt
ref --list # List available note files in note folder

# refe.sh: Edit/open references.txt or other .txt file in note folder
refe # Open references.txt in Vim
refe --open # Open using system default text editor (i.e. Atom, Sublime, TextEdit etc)
refe <keywords> # Search for keywords on line, open in Vim
refe --new notefile2.txt # Create notefile2.txt in note folder
refe notefile2 <keywords> # Search notefile2.txt
refe --list # List available note files in note folder
refe --config # Edit config.txt file. Requires re-running setup.sh
```

## Testing

```bash
bash test/test.sh
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
