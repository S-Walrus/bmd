# bmd
*simple bookmarks manager with dmenu support*

**Dependencies:** `python3`, `dmenu`.

`bmd` stores bookmarks in a human-readable file in `cfg` format typically located at `~/.bookmarks`.
It can look like this:
```
[work]
example_bookmark: https://example.com
another_bookmark: https://example.com

[personal]
youtube: https://youtube.com
```
All bookmarks are organized into groups.

### Usage
```
usage: bmd [-h] [-o NAME] [-l [FOLDER]] [-d]

Simple bookmark manager

optional arguments:
  -h, --help            show this help message and exit
  -o NAME, --open NAME  open a bookmark or a whole group
  -l [GROUP], --list [GROUP]    list all bookmarks or content of GROUP 
  -d, --dmenu           open dmenu to choose a bookmark or a group
```

### TODO
- [ ] automatically create `.bookmarks` file if it doesn't exist
- [ ] avoid parsing bookmarks as a config file
- [ ] support custom bookmarks file
- [ ] support `bmd -l` to list all bookmarks
