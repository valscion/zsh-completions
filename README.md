# zsh-completions for @valscion

HOWTO: https://github.com/zsh-users/zsh-completions/blob/master/zsh-completions-howto.org

To set this up for zsh completions:

```bash
cd /path/to/somewhere
git clone git@github.com:valscion/zsh-completions.git
```

Then open up `~/.zshrc` and add this:

```zsh
fpath=(/path/to/somewhere/zsh-completions $fpath)
```

Then the completions defined in this repository should be active.

If not, you can run this to clear old completions:

```zsh
rm -f ~/.zcompdump
compinit
```
