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
usage: bmd [-h] [-o QUERY] [-l [SECTION]] [-d] [-a GROUP NAME URL] [-c PATH]

Simple bookmark manager

optional arguments:
  -h, --help            show this help message and exit
  -o QUERY, --open QUERY
                        open a bookmark or a group
  -l [SECTION], --list [SECTION]
                        list bookmarks
  -d, --dmenu           open dmenu
  -a GROUP NAME URL, --add GROUP NAME URL
                        add a bookmark
  -c PATH, --config PATH
                        specify data file
```

### TODO
- [x] automatically create `.bookmarks` file if it doesn't exist
- [x] avoid parsing bookmarks as a config file
- [x] support custom bookmarks file
- [x] support `bmd -l` to list all bookmarks
- [x] support `bmd -a` to add a bookmark
