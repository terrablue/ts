# themer -- modern theme switcher for *nix

## installation

Clone this repository into `~/.config/themer`.

`git clone https://github.com/terrablue/themer ~/.config/themer`

Check out the branch corresponding to the theme of your choice.

`cd ~/.config/themer && git checkout nord`

## themes

|name (branch name)|website                  |repos                       |
|------------------|-------------------------|----------------------------|
|nord              |https://www.nordtheme.com|https://github.com/nordtheme|

## configuration

Switching between themes works by adding an include directive to each program.

### alacritty

```toml
import = [
  "~/.config/themer/alacritty.toml",
]
```

## license

All original content is licensed MIT.

All theme content was copied unmodified and retains its original license(s).
