# Tree Emoji CLI

List contents of directories in tree-like 🌳 format with Emojis 📁📄🖼️

Tree-emoji-cli is a recursive directory listing program that produces a depth indented listing of files. With no arguments, tree lists the files in the current directory. When directory arguments are given, tree lists all the files and/or directories found in the given directories each in turn with emojis. Upon completion of listing all files/directories found, tree returns the total number of files and/or directories listed.

## Example

cmd:

```
tree -l 2 -o output.txt
```

result:

```
D:\Sandoche\00 - Projects\Producthunt-floating-prompt
├── 📁  lib
|  ├── 📄  producthunt-floating-prompt.js
|  └── 📄  producthunt-floating-prompt.min.js
├── 📄  LICENSE
├── 🖼️  logo.gif
├── 📄  package-lock.json
├── 📄  package.json
├── 📄  README.md
├── 📁  src
|  ├── 📄  floatingPrompt.js
|  └── 📄  index.js
├── 📁  test
|  ├── 📄  index.html
|  ├── 📄  index.spec.js
|  └── 📄  mocha.opts
├── 📄  webpack.config.js
└── 📄  yarn.lock

directory: 636 file: 14 
```

## Install

```
npm install -g tree-emoji-cli
```

## Usage

use the command `tree` or `treee` (to avoid confliction with system command)

**NOTE: use `treee` instead of `tree` on windows system.**

``
tree/treee
``

#### Use --help to list help info.

``
tree --help
``

#### Specify the level of path (how deep to scan).

use `-l levelNumber` to specify the path level.

```
tree -l 2
```

#### Output result to a file

use `-o outputFilePath` to specify the output file.

```
tree -l 2 -o out.txt
```

#### Show directory only

use `-d` to show directories only.

```
tree -l 2 -o out.txt -d
```

#### Other arguments

see [Options](#options).

#### FOR WINDOWS USERS

you should just use the `treee` command as `tree` has been already taken by windows system.

```
treee -l 2 -o out.txt -d
```

## Options

* --help: outputs a verbose usage listing.
* --version: outputs the version of tree-emoji-cli.
* --debug: show debug info.
* --fullpath: prints the full path prefix for each file.
* --ignore: ignores directory or file you specify - accepts arrays as comma-delimited strings: `'node_modules/, .git/, .gitignore'`
* --link: follows symbolic links if they point to directories, as if they were directories. Symbolic links that will result in recursion are avoided when detected.
* --noreport: omits printing of the file and directory report at the end of the tree listing and omits printing the tree on console.
* -a: all files are printed. By default tree does not print hidden files (those beginning with a dot '.'). In no event does tree print the file system constructs '.' (current directory) and '..' (previous directory).
* -d: list directories only.
* -f: append a '/' for directories, a '=' for socket files and a '|' for FIFOs.
* -i: makes tree not print the indentation lines, useful when used in conjunction with the -f option.
* -l: max display depth of the directory tree.
* -o: send output to filename.

## Credits
This library has been forked from https://github.com/MrRaindrop/tree-cli


## Buy me a beer 🍺
If you like this project, feel free to donate:
* Paypal: https://www.paypal.me/kanbanote
* Bitcoin: 19JiNZ1LkMaz57tewqJaTg2hQWH4RgW4Yp
* Ethereum: 0xded81fa4624e05339924355fe3504ba9587d5419
* Monero: 43jqzMquW2q989UKSrB2YbeffhmJhbYb2Yxu289bv7pLRh4xVgMKj5yTd52iL6x1dvCYs9ERg5biHYxMjGkpSTs6S2jMyJn
* Motive: MOTIV-25T5-SD65-V7LJ-BBWRD (Get Motive Now: https://motive.network)