# Domain list
This is a collection of all the domains for different services

## Remove comments from file
`grep -v '#' filename`

## Automatically generated copies
The GitHub Actions workflow runs on pushes to `main` and can also be run
manually from the Actions tab. It commits copies to `clean/`, removing every
line containing `#` anywhere while preserving all other lines, including blank
lines. Original files are unchanged.

All tracked files are copied except `readme.md`, `.github/`, and `clean/`.
Deleted source files are also removed from `clean/`. The workflow needs
permission to push to `main`; branch protection rules may prevent this.

## DNS commands
`sudo resolvectl monitor`