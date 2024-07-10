# ts – theme switcher for *nix

## installation

Clone this repository into `~/.config/ts`.

`git clone https://github.com/terrablue/ts ~/.config/ts`

Check out the branch corresponding to the theme of your choice.

`cd ~/.config/ts && git checkout nord`

## themes

|name (branch)   |website                  |repos                        |
|----------------|-------------------------|-----------------------------|
|nord            |https://www.nordtheme.com|https://github.com/nordtheme |
|catppuccin mocha|https://catppuccin.com   |https://github.com/catppuccin|

## configuration

Switching between themes works by adding an include directive to each program.

### alacritty

Add to your alacritty TOML configuration.

```toml
import = [
  "~/.config/ts/alacritty.toml",
]
```

### dircolors

Add to your shell configuration

```sh
eval $(dircolors ~/.config/ts/dir_colors)
```

### neovim (nvchad)

Add it to `~/config/nvim/lua/chadrc.lua`

```lua
local theme = dofile(os.getenv("HOME") .. "/.config/ts/nvchad.lua")

return {
  ui = {
    theme = theme,
  }
}
```

## license

All original content is licensed MIT.

All theme content was copied unmodified and retains its original license(s).
