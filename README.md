```
New-Item -Path <SymbolicLink Path> -Value <Source Path> -ItemType SymbolicLink -Force
New-Item -ItemType SymbolicLink -Path "Link" -Target "Target" -Force

# example

New-Item -ItemType Junction -Path "Link" -Target "Target"
New-Item -ItemType Junction -Path "$env:LocalAppData\nvim" -Target "nvim" -Force
New-Item -Path $env:LocalAppData\nvim -Value nvim -ItemType SymbolicLink -Force
```

```
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm

ln -s $HOME/dotfiles/nvim $HOME/.config/nvim
ln -s $HOME/dotfiles/.tmux.conf $HOME/.tmux.conf
```