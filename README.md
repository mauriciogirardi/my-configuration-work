## ZSH

```bash
    # 01 install ZSH
    sudo apt install zsh -y

    # 02 install POWERLINE
    sudo apt install powerline fonts-powerline

    # 03
    chsh -s /bin/zsh

    # 04 Install oh-my-zsh via curl
    sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

    # 05 Zsh Syntax Highlighting
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
    
     # 06 Zsh Auto Suggestions
     git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

    # 07 Spaceship Prompt
    git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1

        # Link
        ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"

    # 04 Edit .zshrc
    code ~/.zshrc

        # Change
        ZSH_THEME="spaceship"
        plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

```

### Links

- [Oh My ZSH](https://ohmyz.sh/)
- [Spaceship Prompt](https://github.com/spaceship-prompt/spaceship-prompt)
- [Zsh Auto Suggestions](https://github.com/zsh-users/zsh-autosuggestions)
- [Zsh Syntax Highlighting](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md/)