# My personal dotfiles

## dotfiles for Windows

* `nvim`

Create `nvim` configuration in `$env:LocalAppData\nvim`. You can git clone dotfiles in git and create a directory junction with the following command.

```pwsh
New-Item -ItemType Junction -Path "$env:LocalAppData\nvim" -Target $PWD\nvim -Force
```

## dotfiles for Linux

* `nvim`

```shell
ln -s $HOME/dotfiles/nvim $HOME/.config/nvim
```

* `tmux`

```shell
ln -s $HOME/dotfiles/.tmux.conf $HOME/.tmux.conf

# install tmux plugin manager
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm

```
