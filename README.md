# wookiee-macbook-setup
Set of scripts or commands I use to setup my Macbook for development. Eventually, this all could be part of an Ansible playbook and executed from there. But baby steps!


# Setup

<details>
    <summary>Upgrade MacOS Terminal</summary>

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

    Now set the theme in your `~/.zshrc` file. For example, `nano ~/.zshrc` and for `ZSH_THEME` set the value to `powerlevel10k/powerlevel10k`

    8) Configure PowerLevel10k

    Close and open iTerm2 and then follow the prompts. If you need to re-run the prompts then execute `p10k configure`

    9) Configure VS Code

    If like to use the terminal within VSCode then you will need to make change to the font to support some of the Powerline features.

    In VS Code do the following:

    - Hit `Cmd+Shift+P`
    - Type `Prefrence: Open Settings (JSON)`, hit Enter
    - In that file include the following:

    ```
    {
        "terminal.integrated.fontFamily": "Cascadia Code PL",
        "editor.fontFamily": "Cascadia Code PL"
    }
    ```
</details>

<details>
    <summary>Installing Python3</summary>

    All credit goes to J Vats and their post here: https://medium.com/geekculture/installing-python-3-x-development-environment-on-macos-a64c0141b20c

    1. Install Xcode from the App Store

    2. Install Python3

    ```zsh
    brew install python
    ```

    3. Check version installed

    ```zsh
    ❯ python3 --version
    Python 3.8.9
    ```

    4. (Optional) Store all virtual environments in one location

    For me that's in my `Development` folder

    ```zsh
    mkdir python-virtual-environments && cd python-virtual-environments
    ```
</details>

<details>
    <summary>Installing NodeJS</summary>

</details>
