# Stata language support in Visual Code
[![Installs!](https://img.shields.io/apm/dm/language-stata.svg?style=flat-square)](https://atom.io/packages/language-stata)
[![Version!](https://img.shields.io/apm/v/language-stata.svg?style=flat-square)](https://atom.io/packages/language-stata)
[![License](https://img.shields.io/apm/l/language-stata.svg?style=flat-square)](https://github.com/kylebarron/language-stata/blob/master/LICENSE)

[![GitHub stars](https://img.shields.io/github/stars/kylebarron/language-stata.svg?style=social&label=Star)](https://github.com/kylebarron/language-stata)
[![GitHub forks](https://img.shields.io/github/forks/kylebarron/language-stata.svg?style=social&label=Fork)](https://github.com/kylebarron/language-stata)

#### Stata syntax highlighting in Visual Code, built from the ground up.

Note: This is a new package that replaces the [previous](https://github.com/benwhalley/atom-language-stata) syntax highlighter. Please add [issues](https://github.com/kylebarron/language-stata/issues) for any bugs, comments, or suggestions.

## Features

This package highlights:
- System commands, functions, and function arguments
- Macros, both global and local
    - Accurately colors nested macros and escaped macros in strings when you want the inner macro to evaluate at runtime
- Regular expressions

Other nice features:
- Alerts you if your variable name is illegal, i.e. if your variable name is more than 32 chars, starts with a number, or is a reserved name.
- Alerts you if you have any text other than } on a line ending a foreach/forvalues/if/else command
- Local macro back tick autocompletion. When you write a `, Visual Code automatically fills in a ' after your cursor
- Makes it easy to spot incorrect nesting of compound quotes
- Support for programming ligatures for all valid Stata syntax for fonts that support them, like the [Fira Code](https://github.com/tonsky/FiraCode) font.
- Highlights [Docblockr](https://atom.io/packages/docblockr)-style keywords inside comments (anything like `@Note`)

## Installation

To install, do one of the following:
- Go to Preferences/Settings > Install > Packages; and then search for "language-stata-plus"
- At the command line, type `apm install language-stata-plus`

## Running Code

This package doesn't have the capabilities to run your code in Stata. If you're using Linux, you can use my [scripts](https://github.com/kylebarron/stata-autokey) with the [Autokey](https://github.com/autokey-py3/autokey) automation utility to quickly run selections of your files in a graphical session of Stata.

You might also be interested in trying to port Atom's `script` or `stata-exec` packages.