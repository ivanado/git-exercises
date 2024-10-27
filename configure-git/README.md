
## Git Initial Configuration

To make sure the Git configuration is correct, run the following

```bash
git config --list
```

The output should contain values for [`user.email`](http://user.email) and [`user.name`](http://user.name) properties.

If the props are not set, use the following commands to add your Git name and email to the global configuration

```bash
git config --global user.name "Your Name"
git config --global user.email your@email.com
```

### Editor setup
Git uses VIM editor by default to edit the files  e.g. to edit the message of a commit you create.
VIM has a steep learning curve, so you might use another tool.

If you want to use the cli based editor nano:
```bash 
git config --global core.editor nano
```

You can use notepad editor in Windows:
```bash 
git config --global core.editor notepad
```