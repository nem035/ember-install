# Ember-Install

Bash script to install/uninstall ember-cli.

## Scripts
- [ember-install](https://github.com/nem035/ember-install/blob/master/ember-install)
  - script that uninstalls current ember cli, if one is installed, and installs the provided version (or latest if nothing is provided)
     
     ```bash
     # install ember cli
     # if you don't specify a version, ember-install will use the latest
     ember-install <version>
    ```
- [ember-uninstall](https://github.com/nem035/ember-install/blob/master/ember-uninstall)
  - Script that uninstalls current ember cli
  
    ```bash
    # uninstall ember cli
    ember-uninstall
    ```

## Installation

Clone the repo and remove the git tracking:

```bash
git clone git@github.com:nem035/ember-install.git
cd ember-install
rm -rf .git
```

Of course one can just download the raw scripts as well.

Don't forget to make the scripts executable

```bash
chmod +x ember-install
chmod +x ember-uninstall
chmod +x print_utils
```

Modify your path to add the directory with `ember-install` scripts:

- Bash:

  ```bash
  echo 'export PATH=$PATH:/{{path_to_ember-install}}' >> ~/.bashrc
  ```

- Zsh

  ```bash
  echo 'export PATH=$PATH:/{{path_to_ember-install}}' >> ~/.zshrc
  ```
  
Assuming you are inside the `ember-install` directory, you can use `$(pwd)` instead of `{{path_to_ember-install}}`:

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
