# wookiee-macbook-setup
Set of scripts or commands I use to setup my Macbook for development. Eventually, this all could be part of an Ansible playbook and executed from there. But baby steps!


# Setup

### Upgrade MacOS Terminal

1) Install [Homebrew](https://brew.sh/)

```zsh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2) Install iTerm2

```zsh
brew install --cask iterm2
```
3) Install git

```zsh
brew install git
```

4) Install [Oh-My-Zsh](https://ohmyz.sh/)

```zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

5) Install [Powerline](https://github.com/powerline/powerline) Fonts <font size="1"> (*I prefer [Cascadia Code](https://github.com/microsoft/cascadia-code) from Microsoft*)</font>

Installation instruction font here: https://github.com/microsoft/cascadia-code/wiki/Installing-Cascadia-Code

6) Update iTerm2 Preferences

- Go to Preferences (cmd + ,)
- Click Profile Tab
- Add a new profile (example: *yourname*)
- Delete the `Default` profile
- Select the `Text` tab
- Under `Font` section serach for `Cascadia Code PL`
- Check off `Use Ligatures`
- Now select `Session` tab
- At the very bottom, check off `Status bar enabled`
- Click `Configure Status bar`
- I like to use CPU, RAM, and Network
- Click `Ok`
- Exit out of Preferences and then reload iTerm2

Other configuration considerations, [Color Schemes](https://awesomeopensource.com/project/mbadolato/iTerm2-Color-Schemes)

7) Install and Setup [Oh-My-ZSH Theme](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes) <font size="1"> (*I prefer powerlevel10k*)</font>

```zsh
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```

