# My tmux config

This is my tmux config, with the catpuccin theme. It supports the script `tmux-sessionizer` built by the great SWE [The Primeagen](https://github.com/theprimeagen)

# Installation

1. Install TPM

```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

2. Clone the repository and create syslink for the config

```bash
git clone https://github.com/omardoescode/tmux-config.git
ln tmux-config/.tmux.conf ~/.tmux.conf # Create symlink for the config
ln tmux-config/tmux-sessionizer ~/.local/bin/tmux-sessionizer # Create symlink for the tmux sessionizer
```

3. Add `tmux-sessionizer` path to `$PATH`

Add the path `.local/bin` to your `$PATH` global variable.

```bash
export PATH=$PATH:$HOME/.local/bin
```

4. Add aliases (optional)

   You can also add aliases for tmux

```bash
# tmux
alias t='tmux'
alias td='t detach'
alias ts='tmux neww tmux-sessionizer'
```

5. Setup `tmux-sessionizer`

   Open tmux-sessionizer file and edit the paths in which you want `tmux-sessionizer` to work
