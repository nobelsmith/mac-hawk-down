# mac-hawk-down
Init script for mac to get all the goods installed

Brew
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

VS Code
```bash
brew install - cask visual-studio-code
```

Nerd Fonts
```bash
brew tap homebrew/cask-fonts
brew search '/font-.*-nerd-font/' | awk '{ print $1 }' | xargs -I{} brew install - cask {} || true
```

Alacritty
```bash
brew install alacritty
```

Neovim
```bash
brew install neovim
```

Oh My Zsh
```bash
brew install zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
plugins

autojump
```bash
brew install autojump
```
Add the following line to your ~/.bash_profile or ~/.zshrc file:
```bash
[ -f $HOMEBREW_PREFIX/etc/profile.d/autojump.sh ] && . $HOMEBREW_PREFIX/etc/profile.d/autojump.sh
```

zsh-syntax-highlighting
```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
Add zsh-syntax-highlighting to your ~/.zshrc file plugins

zsh-autosuggestions
```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
Add zsh-syntax-highlighting to your ~/.zshrc file plugins
