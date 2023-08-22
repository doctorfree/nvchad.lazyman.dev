---
layout: post
icon: fas fa-info-circle
order: 3
toc: true
post_style: page
---

## NvChad Features

See [https://nvchad.com/docs/features](https://nvchad.com/docs/features)
for the latest on current features of NvChad based Neovim configurations.

## Inbuilt features

- NvChad is built upon its personal plugins and many general neovim plugins, below are the features that are provided by nvchad plugins **( their ui plugin, base46, extensions, nvterm, nvim-colorizer )**

### Base46

- Base46 is NvChad's highlight performant theming plugin and has many ported themes ( around 57+ ).

#### How it works?

- Gets highlight groups 
- Do some computations i.e check for overriden highlight groups, new highlight groups, theme overrides, custom user themes etc.  
- Now base46 compiles all of that into bytecode.
- Integration files aren't loaded by default, for example highlight group for telescope, nvimtree etc are put into different files.
- highlight groups are lazyloaded i.e you load them when needed 
- **example : dofile(vim.g.base46_cache .. "cmp")**
- In the below video you can see that the chadrc file's ( user config ) UI related options reload on the fly 

<div class="iframe-container">
  <iframe src="https://www.youtube.com/embed/xytzreFq_us" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allow="fullscreen"></iframe>
</div>

### Theme switcher

- A theme switcher with telescope.nvim which reloads theme on the fly using base46 plugin + plenary.nvim.

<div class="iframe-container">
 <iframe  src="https://www.youtube.com/embed/wt7IX8ojMrs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"  allow="fullscreen;"></iframe>
</div>

### Statusline 

- They have their own statusline module ( their UI Plugin ) which has 4 statusline styles

![nvchad statusline](https://nvchad.com/features/statuslines.webp)

### Tabufline

- NvChad's tabufline module ( from UI Plugin ) is a mix of tabline & bufferline. 
- It manages buffers & tabs, buttons in it are clickable
- Each tab will have its own set of buffers stored and the tabufline will show those only.
- Think it like workspaces on Linux/Windows where windows stay in their own workspaces, but in vim buffers from all tabs will be shown in every tab!

<div class="iframe-container">
<iframe src="https://www.youtube.com/embed/V_9iJ96U_k8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allow="fullscreen;"></iframe>
</div>

### Nvterm 

- NvChad's terminal plugin to toggle and run commands in neovim terminal buffer
- Using it with their telescope picker ( :Telescope terms ) to unhide terminal buffers <kbd> leader + pt </kbd>.

<div class="iframe-container">
<iframe src="https://www.youtube.com/embed/3DysWI_6YpQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allow="fullscreen;"></iframe>
</div>


### Dashboard

- Nvdash is NvChad's minimal dashboard module, It's very simple at this stage and will get more features in the future!
- Command to run it `Nvdash`, its disabled on startup, check the default_config.lua for its syntax and override it from chadrc.

![nvdash](https://nvchad.com/features/nvdash.webp)

### NvCheatsheet

- Auto-generated mappings cheatsheet module which has a similar layout to that of CSS's masonry layout.
- It has 2 themes ( grid & simple )

![nvcheatsheet](https://nvchad.com/features/nvcheatsheet.webp)

- command to toggle it : `NvCheatsheet` and mapping `leader + ch`

<div class="iframe-container">
<iframe src="https://www.youtube.com/embed/IljDD4cjgKc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allow='fullscreen;'></iframe>
</div>

## General neovim plugins

- These plugins aren't related to nvchad, we just tweak theme a bit and theme the UI related ones.

### Telescope.nvim

- [Telescope.nvim](https://github.com/nvim-telescope/telescope.nvim) is a highly extendable fuzzy finder over lists. Built on the latest awesome features from neovim core. Telescope is centered around modularity, allowing for easy customization.
- Below are 2 styles of telescope in nvchad ( bordered and borderless )

![telescope](https://nvchad.com/features/telescope.webp)

### Nvim-tree.lua

- [`nvim-tree.lua`](https://github.com/kyazdani42/nvim-tree.lua) is a file explorer tree for Neovim written in Lua.

![nvim tree](https://raw.githubusercontent.com/siduck/dotfiles/all/rice%20flex/nvimtree.png)


### Nvim-cmp

- [`nvim-cmp`](A completion plugin for neovim coded in Lua.) is a completion plugin for neovim coded in Lua.
- Below are some cmp styles in nvchad 

![nvim-cmp](https://nvchad.com/features/cmp.webp)

- Note that thats just the cmp look in everblush theme, there are more 57 themes! You can hide cmp icons, cmpkind txt etc from the user config ( chadrc ) itself! 

### Auto-completion & LSP

- [`nvim-lspconfig`](https://github.com/neovim/nvim-lspconfig) is used along with cmp for completion and [`luasnip`](https://github.com/L3MON4D3/LuaSnip)  + [`friendly-snippets`](https://github.com/rafamadriz/friendly-snippets) for snippet completion! 
<div class="iframe-container">
<iframe src="https://www.youtube.com/embed/oMzMDXA-VO0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allow='fullscreen;'></iframe>
</div>

<br/>

- [`lazy.nvim`](https://github.com/folke/lazy.nvim) - A modern plugin manager for Neovim
- [`whichkey.nvim`](https://github.com/folke/which-key.nvim) - Create key bindings that stick. WhichKey is a lua plugin for Neovim 0.5 that displays a popup with possible keybindings of the command you started typing.
- [`nvim-colorizer.lua`](https://github.com/NvChad/nvim-colorizer.lua) - Fastest Neovim colorizer, hex colors, hsl codes and much more.
- [`nvim-treesitter`](https://github.com/nvim-treesitter/nvim-treesitter) - Nvim Treesitter configurations and abstraction layer, we use it for syntax highlighting & auto-indenting. 
- [`blankline`](https://github.com/lukas-reineke/indent-blankline.nvim) - Indent guides for Neovim i.e indentline plugin.
- [`gitsigns.nvim`](https://github.com/lewis6991/gitsigns.nvim) - Git integration for buffers
- [`nvim-autopairs`](https://github.com/windwp/nvim-autopairs)
- [`comment.nvim`](https://github.com/numToStr/Comment.nvim) - Commenting plugin
- [`mason.nvim`](https://github.com/williamboman/mason.nvim) - Portable package manager for Neovim that runs everywhere Neovim runs. Easily install and manage LSP servers, DAP servers, linters, and formatters.
