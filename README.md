
# Fragments of Time

## Basic

`git init` - creates a local repository

`git add .` - Stages all the files that were changed

`git add <file1> <file2>` - related changes

`git add <file3>` - not related changes

`git commit -m "Accurate Description"` - point in time, changes have been made, and it's very important

## Reviewing your changes

> git **log** - shows all your commit changes

`git log --pretty=oneline <options>`
options include:  
1. `--max-count=2`

2. `--since='time span'`  

3. `--author=<author-name>`

4. `--all`

## Ultimate Log Format - Good to know

`git log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short`

In detail:

- `--pretty="..."` defines the format of the output.
- `%h` is the abbreviated hash of the commit
- `%d` are any decorations on that commit (e.g. branch heads or tags)
- `%ad` is the author date
- `%s` is the comment
- `%an` is the author name
- `--graph` informs git to display the commit tree in an ASCII graph layout
- `--date=short` keeps the date format nice and short