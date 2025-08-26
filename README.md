# 🌳 Nvim Treesitter: Your Go-To Configuration and Abstraction Layer

Welcome to the Nvim Treesitter repository! This project provides configurations and an abstraction layer for using Treesitter with Neovim. If you're looking to enhance your coding experience in Neovim, you're in the right place. 

[![Download Releases](https://img.shields.io/badge/Download%20Releases-Here-blue)](https://github.com/Jumaannjii/nvim-treesitter/releases)

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Supported Languages](#supported-languages)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

Nvim Treesitter aims to provide an easy and efficient way to integrate Treesitter into your Neovim setup. Treesitter is a powerful tool that allows for advanced syntax highlighting and code analysis. With this repository, you can leverage Treesitter's capabilities without dealing with complex configurations.

## Features

- **Easy Setup**: Quickly get started with minimal configuration.
- **Multi-language Support**: Use Treesitter with various programming languages.
- **Enhanced Syntax Highlighting**: Enjoy better code readability and structure.
- **Code Folding**: Fold and unfold code blocks seamlessly.
- **Incremental Parsing**: Benefit from faster updates and lower memory usage.

## Installation

To install Nvim Treesitter, follow these steps:

1. Make sure you have Neovim installed. You can check this by running `nvim --version` in your terminal.
2. Install the Treesitter plugin. You can use a plugin manager like `vim-plug`, `packer.nvim`, or any other manager of your choice.

For example, if you are using `vim-plug`, add the following line to your `init.vim` or `init.lua`:

```vim
Plug 'nvim-treesitter/nvim-treesitter', {'do': ':TSUpdate'}
```

After adding the plugin, run `:PlugInstall` in Neovim.

3. Once installed, download and execute the latest release from the [Releases page](https://github.com/Jumaannjii/nvim-treesitter/releases).

## Configuration

After installation, you need to configure Nvim Treesitter. You can do this in your `init.vim` or `init.lua` file. Here’s a simple configuration example:

```lua
require'nvim-treesitter.configs'.setup {
  ensure_installed = {"lua", "python", "javascript"}, -- List of languages to install
  highlight = {
    enable = true,              -- false will disable the whole extension
    additional_vim_regex_highlighting = false,
  },
  indent = {
    enable = true
  },
}
```

This configuration ensures that Treesitter installs support for Lua, Python, and JavaScript. You can customize the list based on your needs.

## Usage

Once configured, you can start using Nvim Treesitter features. Here are some common commands:

- **Highlighting**: Treesitter will automatically highlight your code based on the configured languages.
- **Folding**: Use `zc` to fold and `zo` to unfold code blocks.
- **Incremental Selection**: Use `gnn` to start selecting a node and `gns` to expand the selection.

## Supported Languages

Nvim Treesitter supports a wide range of programming languages. Some of the popular ones include:

- Lua
- Python
- JavaScript
- TypeScript
- Go
- Rust
- C
- C++
- HTML
- CSS

For a complete list, refer to the [official Treesitter repository](https://github.com/tree-sitter/tree-sitter).

## Contributing

We welcome contributions! If you want to help improve Nvim Treesitter, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes to your forked repository.
5. Create a pull request to the main repository.

Please ensure that your code follows the existing style and includes tests where applicable.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or suggestions, feel free to open an issue on the repository or reach out to the maintainers.

You can also check the [Releases section](https://github.com/Jumaannjii/nvim-treesitter/releases) for the latest updates and downloads.

---

Thank you for using Nvim Treesitter! We hope it enhances your coding experience in Neovim.