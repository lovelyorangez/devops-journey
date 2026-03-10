## 🎮 OverTheWire: Bandit Lab Notes

Completed **Levels 0 through 3**. These levels focused on handling "non-standard" filenames.

### Level 0 → 1: The Dash Filename
* **Problem:** A file named `-` cannot be read with `cat -` because the shell thinks `-` is an option flag.
* **Solution:** Used a relative path to specify the file.
* **Command:** `cat ./-`

### Level 1 → 2: Spaces in Filenames
* **Problem:** Files with spaces like `spaces in this filename`.
* **Solution:** Used double quotes to treat the string as a single argument.
* **Command:** `cat "spaces in this filename"` (or used Tab-completion).

### Level 2 → 3: Hidden Files
* **Problem:** The file was hidden in the `inhere` directory.
* **Solution:** Hidden files in Linux start with a dot (`.`). Standard `ls` doesn't show them.
* **Command:** `ls -a` inside the directory to reveal `.hidden`.
