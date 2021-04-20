# *nginx* config file formatter

This Python script formats *nginx* configuration files in consistent
way, described below:

* all lines are indented in uniform manner, with 4 spaces per level
* neighbouring empty lines are collapsed to at most two empty lines
* curly braces placement follows Java convention
* whitespaces are collapsed, except in comments and quotation marks

## Installation

Python 3.4 or later is needed to run this program. The simplest form
of installation would be copying `nginxfmt.py` to your scripts directory.

You can also clone the repository and symlink the executable:

```
cd
git clone https://github.com/slomkowski/nginx-config-formatter.git
ln -s ~/nginx-config-formatter/nginxfmt.py ~/bin/nginxfmt.py
```

## Usage

```
usage: nginxfmt.py [-h] [-v] [-b] config_files [config_files ...]

Script formats nginx configuration file.

positional arguments:
  config_files          configuration files to format

optional arguments:
  -h, --help            show this help message and exit
  -v, --verbose         show formatted file names
  -b, --backup-original
                        backup original config file
```

## Reporting bugs

Please create issue under https://github.com/slomkowski/nginx-config-formatter/issues.
Be sure to add config snippets to reproduce the issue, preferably:

* snippet do be formatted
* actual result with invalid formatting
* desired result


## Credits

Copyright 2021 Michał Słomkowski. License: Apache 2.0.
