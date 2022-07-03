# poetry-nvim

I needed a way for VIRTUAL_ENV to be set to the one set by [Poetry](https://python-poetry.org/).
Mainly to get LSP stuff to work.

Other plugins (see [alternatives](#left_right_arrow-alternatives)) existed but they did not do what I expected. That is probably explained by me being lazy and being curious on how to write a Neovim plugin with Lua.

## :package: Installation

Install this plugin with your favorite package manager:

### [packer.nvim](https://github.com/wbthomason/packer.nvim)

```lua
use({
    "karloskar/poetry-nvim",
    config = function()
        require("poetry-nvim").setup()
    end
})
```

### [vim-plug](https://github.com/junegunn/vim-plug)

```vim
Plug "karloskar/poetry-nvim"

lua << EOF
    require("poetry-nvim").setup()
EOF
```

## :left_right_arrow: Alternatives

Before making this plugin I looked at:

- [Poet-v](https://github.com/petobens/poet-v)
- [vim-venom](https://github.com/rafi/vim-venom)
