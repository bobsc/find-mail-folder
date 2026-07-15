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

## Examples
% find-mail-fldr bible
[On My Mac]: Rockwall Bible Church
[On My Mac]: Christian Lists/Blue Letter Bible
[On My Mac]: Christian Lists/Back to the Bible
[On My Mac]: Christian Lists/Bible Framework
[On My Mac]: Christian Lists/Redeemer Bible Church
[On My Mac]: Christian Lists/Online Bible
[On My Mac]: Christian Lists/Apostolic Bible - Charles Vanderpool
[On My Mac]: Christian Lists/Messianic Bible
[On My Mac]: Christian Lists/Bible Gateway
[On My Mac]: Christian Lists/Bible Analyzer
[On My Mac]: Christian Lists/BibleMemory.com

% find-mail-fldr "dr dobbs"
[iCloud]: Dr Dobbs

% find-mail-fldr inbox
[txbobsc]: INBOX
[yahoo]: INBOX
[Gmail]: INBOX
[iCloud]: INBOX
[AOL BrCrk]: INBOX
[AOL BobSC]: INBOX

## License
MIT License - Free to use and modify.
