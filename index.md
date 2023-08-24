---
layout: post
title: NvChad Configurations
toc: true
post_style: page
---

## Lazyman Supported NvChad Neovim Configurations

The following are [Lazyman](https://lazyman.dev) supported
[NvChad](https://nvchad.com){:target="_blank"}{:rel="noopener noreferrer"}
based Neovim configurations:

| Lazyman | Supported | NvChad | Neovim | Configs |
| :------ | :-------: | :----: | :----: | ------: |
| [NvChad](https://nvchad.lazyman.dev/posts/NvChad) | [Cpp](https://nvchad.lazyman.dev/posts/Cpp) | [Go](https://nvchad.lazyman.dev/posts/Go) | [Python](https://nvchad.lazyman.dev/posts/Python) | [Rust](https://nvchad.lazyman.dev/posts/Rust) |

Install all Lazyman supported NvChad configurations with the command: `lazyman -i nvchad`

## What is NvChad

[NvChad](https://nvchad.com){:target="_blank"}{:rel="noopener noreferrer"}
is one of the most popular Neovim "distributions"
along with [LazyVim](https://lazyvim.lazyman.dev),
[LunarVim](https://lunarvim.lazyman.dev), and
[AstroNvim](https://astronvim.lazyman.dev). These aren't really distributions,
they do not include Neovim, but that is what they are called. They are more
accurately described as "Neovim configuration frameworks". In most cases they
provide some pre-configuration of plugins as well as an easy way to extend
the base configuration. Note that NvChad, unlike other Neovim configuration
distributions, is not a framework.

A Neovim configuration distribution can be of considerable assistance in managing
the exploding Neovim plugin ecosystem, quickly and easily incorporating
advanced features, and maintaining an up-to-date Neovim configuration.

- NvChad is a neovim config written in lua aiming to provide a base configuration with very beautiful UI and blazing fast startuptime (around 0.02 secs ~ 0.07 secs). We tweak UI plugins such as telescope, nvim-tree, bufferline etc well to provide an aesthetic UI experience. 

- Lazy loading is done 93% of the time meaning that plugins will not be loaded by default, they will be loaded only when required also at specific commands, events etc. This lowers the startuptime and it was like 0.07~ secs tested on an old pentium machine 1.4ghz + 4gb ram & HDD.

- NvChad isn't a framework! It's supposed to be used as a "base" config, so users can tweak the defaults well, and also remove the things they don't like in the default config and build their config on top of it. Users can tweak the entire default config while staying in their custom config (lua/custom dir). This is the control center of the user's config and gitignored so the users can stay up-to-date with NvChad's latest config (main branch) while still controlling it with their chadrc (file that controls entire custom dir).

Features that distinguish NvChad include:

- Really great `base46` plugin enables easy theme/colorscheme management
- Includes an impressive mappings `cheatsheet`
- `ui` plugin and `nvim-colorizer`

Read our overview and comparison of
[Neovim configuration distributions](https://lazyman.dev/posts/Configuration-Distributions).

## Showcase

See the [Showcase section](https://nvchad.lazyman.dev/showcase) for screenshots.

## UI related plugins used

<details><summary> <b>Images (Click to expand!)</b></summary>

<h3> Nvim-tree.lua </h3>

Fast file tree:

<kbd><img src="https://nvchad.com/features/nvimtree.webp"></kbd>

<h3> Telescope-nvim </h3>

A fuzzy file finder, picker, sorter, previewer and much more:

<kbd><img src="https://nvchad.com/features/telescope.webp"></kbd>

<h3> Their own statusline written from scratch  </h3>

[NvChad UI](https://github.com/NvChad/ui){:target="_blank"}{:rel="noopener noreferrer"}

<kbd><img src="https://nvchad.com/features/statuslines.webp"></kbd>

<h3> Tabufline (their own pertab bufferline) </h3>

<kbd><img src="https://nvchad.com/features/tabufline.webp"></kbd>
- Here's a [video](https://www.youtube.com/watch?v=V_9iJ96U_k8&ab_channel=siduck){:target="_blank"}{:rel="noopener noreferrer"} that showcases it.

<h3> NvCheatsheet ( their UI Plugin ) </h3>
<kbd> <img src="https://nvchad.com/features/nvcheatsheet.webp"/></kbd>

</details>

## Plugins list

- Many beautiful themes, theme toggler by their [base46 plugin](https://github.com/NvChad/base46){:target="_blank"}{:rel="noopener noreferrer"}
- Inbuilt terminal toggling & management with [Nvterm](https://github.com/NvChad/nvterm){:target="_blank"}{:rel="noopener noreferrer"}
- NvChad updater, hide & unhide terminal buffers with [NvChad extensions](https://github.com/NvChad/extensions){:target="_blank"}{:rel="noopener noreferrer"}
- Lightweight & performant ui plugin with [NvChad UI](https://github.com/NvChad/ui){:target="_blank"}{:rel="noopener noreferrer"} It provides statusline modules, tabufline ( tabs + buffer manager) , beautiful cheatsheets and much more!
- File navigation with [nvim-tree.lua](https://github.com/kyazdani42/nvim-tree.lua){:target="_blank"}{:rel="noopener noreferrer"}
- Beautiful and configurable icons with [nvim-web-devicons](https://github.com/kyazdani42/nvim-web-devicons){:target="_blank"}{:rel="noopener noreferrer"}
- Git diffs and more with [gitsigns.nvim](https://github.com/lewis6991/gitsigns.nvim){:target="_blank"}{:rel="noopener noreferrer"}
- NeoVim Lsp configuration with [nvim-lspconfig](https://github.com/neovim/nvim-lspconfig){:target="_blank"}{:rel="noopener noreferrer"} and [mason.nvim](https://github.com/williamboman/mason.nvim){:target="_blank"}{:rel="noopener noreferrer"}
- Autocompletion with [nvim-cmp](https://github.com/hrsh7th/nvim-cmp){:target="_blank"}{:rel="noopener noreferrer"}
- File searching, previewing image and text files and more with [telescope.nvim](https://github.com/nvim-telescope/telescope.nvim){:target="_blank"}{:rel="noopener noreferrer"}
- Syntax highlighting with [nvim-treesitter](https://github.com/nvim-treesitter/nvim-treesitter){:target="_blank"}{:rel="noopener noreferrer"}
- Autoclosing braces and html tags with [nvim-autopairs](https://github.com/windwp/nvim-autopairs){:target="_blank"}{:rel="noopener noreferrer"}
- Indentlines with [indent-blankline.nvim](https://github.com/lukas-reineke/indent-blankline.nvim){:target="_blank"}{:rel="noopener noreferrer"}
- Useful snippets with [friendly snippets](https://github.com/rafamadriz/friendly-snippets){:target="_blank"}{:rel="noopener noreferrer"} plus [LuaSnip](https://github.com/L3MON4D3/LuaSnip){:target="_blank"}{:rel="noopener noreferrer"}
- Popup mappings keysheet [whichkey.nvim](https://github.com/folke/which-key.nvim){:target="_blank"}{:rel="noopener noreferrer"}

<div align="center">
  <p align="center">
    <a href="https://ronrecord.com" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="domain"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/domain.png"
    /></a>
    <a href="https://www.reddit.com/user/No-Blackberry-3160" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="reddit"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/reddit.png"
    /></a>
    <a href="https://github.com/doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="github"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/github.png"
    /></a>
    <a href="https://gitlab.com/doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="gitlab"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/gitlab.png"
    /></a>
    <a href="https://twitter.com/ronrecord" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="twitter"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/twitter.png"
    /></a>
    <a href="https://youtube.com/c/doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="youtube"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/youtube.png"
    /></a>
    <a href="https://linkedin.com/in/ronrecord" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="linkedin"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/linkedin.png"
    /></a>
    <a href="https://instagram.com/doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="instagram"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/instagram.png"
    /></a>
    <a href="https://noc.social/@doctorwhen" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="mastodon"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/mastodon.png"
    /></a>
    <a href="https://en.wikipedia.org/wiki/User:Doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="wikipedia"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/wikipedia.png"
    /></a>
  </p>
</div>
