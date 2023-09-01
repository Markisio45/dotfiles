# kitty Terminal running zsh

Fot this configuration you have to follow the next steps:

## 1. Download the repo and move the content on the kitty folder into your kitty config folder.
> It is usually located on `~/.config/kitty`

## 2. Replace the .zshrc in your ~/ directory with the .zshrc provided on this repo.

## 3. Fixing Errors

As you can see if you run the terminal now, there will be shown some errors on top of ther terminal, showing that there are missing files.

### `zsh-syntax-highlighting` and `zsh-autosuggestions` errors

We can fix `zsh-syntax-highlighting` and `zsh-autosuggestions` by running the following command

> sudo apt install zsh-syntax-highlighting zsh-autosuggestions

Use apt or any other package manager.

### `sudo.plugin.zsh` error

Download the file from this repository ohmyzsh/ohmyzsh on github
> https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/plugins/sudo/sudo.plugin.zsh

Set the file on the directory `/usr/share/zsh-sudo`


### Installing powerlevel10k

Go to the GitHub repository romkatv/powerlevel10k and execute the command from Manual Installation:
> git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
> echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc

we can download font from the next resources:

> http://fontlot.com/downfile/5baeb08d06494fc84dbe36210f6f0ad5.105610
> https://www.dropbox.com/s/hrkub2yo9iapljz/icommon.zip?dl=0


## 4. Upgrading `cat` and `ls` commands

We are going to replace the `cat` command with `bat` and `ls` with `lsd`

Install lsd:
> Go to: `https://github.com/Peltoche/lsd/releases` and download the .deb
> sudo dpkg -i lsd_0.23.1_amd64.deb 

Install bat
> sudo apt install bat
