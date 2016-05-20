#Ember-Install

Bash script to install/uninstall ember-cli.

## Installation

Clone the repo and make it your own:

```bash
  git clone git@github.com:nem035/ember-install.git
  cd ember-install
  rm -rf .git && git init
```
Make the scripts executable

```bash
  chmod +x ember-install
  chmod +x ember-uninstall
  chmod +x print_utils

  # or chmod +x *
```

Modify your path to add the directory with `ember-install` scripts:

```bash
  export PATH=$PATH:/ember-install
```

## Usage

```bash
  # if you don't specify a version, ember-install will use the latest
  ember-install <version>
```

## Example
```bash
15:31:12 › ember-install 2.4.3

#########################################################
Uninstalling Ember-CLI

version: 2.4.2 node: 0.12.7 os: darwin x64
- abbrev@1.0.7 node_modules/ember-cli/node_modules/abbrev
- acorn@1.2.2 node_modules/ember-cli/node_modules/acorn
... # removed output for brevity

Done.

#########################################################
Cleaning NPM cache...

... # removed output for brevity

Done.

#########################################################
Cleaning Bower cache...

... # removed output for brevity

Done.

#########################################################
Installing ember@2.4.3 ...

... # removed output for brevity

Done.
```