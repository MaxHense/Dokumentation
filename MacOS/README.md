## iterm2
You can import the iterm2 profile into the profiles. In iterm2
`Profiles > Open Profiles > Edit Profiles > Other Actions > Import Profiles > *choose the .json-file*`
Afterwards go
`Profiles > Open Profiles > *choose the new Profile, delete the old one*`

## brew
In a single user environment, it is possible to install with the normal homebrew script

In a multiple user environment add new brew to user:
```
cd $HOME
git clone https://github.com/Homebrew/brew.git
./brew/bin/brew tap homebrew/core
```

add brew to Path
`PATH=$HOME/brew/bin:$PATH`

## aerospace
To implement aerospace, just copy the aerospace.toml into .aerospace.toml in the homefolder of the user

## ZSH
zsh is installed on mac. Add an zshrc

`touch .zshrc`

add .oh-my-zsh

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

add powerlevel10k

`git clone --depth=1 https://github.com/romkatv/powerlevel10k.git "${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k"`

add all plugins

```
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
git clone https://github.com/zdharma-continuum/fast-syntax-highlighting.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/fast-syntax-highlighting
git clone --depth 1 -- https://github.com/marlonrichert/zsh-autocomplete.git $ZSH_CUSTOM/plugins/zsh-autocomplete
```

copy the zshrc into the folder

add plugins to zsh

plugins=(
  git
  zsh-autosuggestions
  zsh-syntax-highlighting
  fast-syntax-highlighting
  zsh-autocomplete
 )

## Vim

## files (Ordner)

Zum Abspeichern der Daten wird ein passwortgeschütztes zip file verwendet. Passwort hierzu ist auffindbar im keepass.
