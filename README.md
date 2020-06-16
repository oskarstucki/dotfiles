# dotfiles

Dotfiles for sensible OS X life. Heavily influenced by
https://github.com/mathiasbynens/dotfiles.

Installing guide from [Sirile's blog](http://sirile.github.io/2015/01/26/setting-up-mac.html) for more information about installing.

## Install brew

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

## Clone the dotfiles

```
git clone https://github.com/oskarstucki/dotfiles.git ~/.dotfiles
```

## Install the default packages with a bundle

```
cd .dotfiles
brew bundle
```

## Run RCM

RCM links the files in the .dotfiles folder to the user’s home directory. This way they can easily be maintained with git in their own folder without the home folder becoming too complex with .gitignore.

```
rcup rcrc
rcup -f
```

### Make GNU bash default shell

```
echo "/usr/local/bin/bash" | sudo tee -a /etc/shells
chsh -s /usr/local/bin/bash
```

## Install nvm

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.35.3/install.sh | bash

```
