# Linux

List of contents:

- [Arch Linux](#ArchLinux)
- [Useful Commands](#usefulCommands)

----

## [Arch Linux](https://www.archlinux.org)

----

## Useful Commands

----

### Display Disk Usage while excluding .git and node_modules directories

```bash
ncdu --color dark -rr -x --exclude .git --exclude node_modules
```

### Edit command line in editor

I'm using zsh, so pressing ```<ALT-e>``` while in ```INSERT```-mode is much more pleasant than trying to press ```<ESC>``` with your small little finger.

### Replace insecure git URLs with HTTPS or SSH

in your ```.gitconfig``` file you may use one or the other (```HTTPS``` or ```SSH```), but not both

```
# replace with HTTPS
[url "https://github.com"]
     insteadOf = git://github.com

# replace with SSH
[url "git@github.com"]
     insteadOf = git://github.com

# replace HTTPS with SSH
[url "git@github.com:"]
     insteadOf = https://github.com/
```

or on the command line

rewrite any ```git://``` URL *only* with ```https://```
```bash
git config --global url."https://github.com".insteadOf git://github.com
```

or rewrite any ```git://``` URL *only* with ```git@```
```bash
git config --global url."git@github.com".insteadOf git://github.com
```

or replace ```https://github.com/``` URL with ```git@github.com:```
```bash
git config --global url."git@github.com:".insteadOf https://github.com/
```
