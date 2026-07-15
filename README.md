# find-mail-folder
Find a particular mail folder in the hiearchy of accounts and folders in Mac Mail

A lightweight, blazing-fast Bash utility to instantly find specific email folders hidden deep within the Apple Mail directory hierarchy on macOS. 

This tool completely bypasses broken or corrupted native Apple Mail / Spotlight search indexing by querying the backend `.mbox` structure directly.

## Features
- Finds hidden or nested subfolders without expanding your entire mailbox tree.
- Dynamically resolves cryptic macOS UUID account names into human-readable names.
- Colors and highlights matches directly in the terminal interface.

## Installation

1. Clone or download this repository.
2. Make the script executable:
   ```bash
   chmod +x find-mail-fldr
   ```
3. Move it to your local binary path to run it globally from anywhere:
   ```bash
   mv find-mail-fldr /usr/local/bin/
   ```

## Usage

Simply pass the name (or part of the name) of the folder you want to locate:

```bash
find-mail-fldr "Alpha"
find-mail-fldr "Project Alpha"
```

## License
MIT License - Free to use and modify.
