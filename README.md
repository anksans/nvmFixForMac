# nvmFixForMac
nvm.sh:295: parse error near `}'


mkdir ~/.nvm

https://github.com/nvm-sh/nvm/archive/v0.33.11.tar.gz
extract and move contents out of it in ~/.nvm

mv  -r nvm-0.33.11/* ~/.nvm

```sh
export NVM_DIR="$HOME/.nvm" && (bash "$NVM_DIR/nvm.sh")
```

Now add these lines to your `~/.bashrc`, `~/.profile`, or `~/.zshrc` file to have it automatically sourced upon login:
(you may have to add to more than one of the above files)

```sh
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
```
