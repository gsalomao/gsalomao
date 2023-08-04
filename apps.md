# Unix Applications

## [bat](https://github.com/sharkdp/bat)

A `cat` clone with syntax highlighting and Git integration.

![bat](https://camo.githubusercontent.com/c436c206f2c86605ab2f9fb632dd485afc05fccbf14af472770b0c59d876c9cc/68747470733a2f2f692e696d6775722e636f6d2f326c53573452452e706e67)

#### Installation

```zsh
brew install bat
```

#### Configuration

```zsh
alias cat='bat --theme=Dracula'
alias bathelp='bat --plain --language=help'

help() {
    "$@" --help 2>&1 | bathelp
}
```

## [lsd](https://github.com/lsd-rs/lsd)

The next gen file listing command. Backwards compatible with `ls`.

![lsd](https://raw.githubusercontent.com/Peltoche/lsd/assets/screen_lsd.png)

#### Installation

```zsh
brew install lsd
```

#### Configuration

```zsh
alias ls='lsd --date relative --group-dirs=first --header'
alias l='ls -l'
alias la='ls -a'
alias lla='ls -la'
alias lt='ls --tree'
```

## [delta](https://github.com/dandavison/delta)

A viewer for `git` and `diff` output.

![delta](https://user-images.githubusercontent.com/52205/87230973-412eb900-c381-11ea-8aec-cc200290bd1b.png)


#### Installation

```zsh
brew install git-delta
```

#### Configuration

```gitconfig
[core]
    pager = delta

[interactive]
    diffFilter = delta --color-only

[delta]
    navigate = true    # use n and N to move between diff sections
    light = false      # set to true if you're in a terminal w/ a light background color (e.g. the default macOS terminal)
    side-by-side = true

[merge]
    conflictstyle = diff3

[diff]
    colorMoved = default
```

## [dust](https://github.com/bootandy/dust)

A more intuitive version of `du` written in Rust.

![dust](https://user-images.githubusercontent.com/200613/90223722-e0c2e980-de0e-11ea-8c75-343273fed6f3.png)


#### Installation

```zsh
brew install dust
```

#### Configuration

```zsh
alias du='dust'
```

## [duf](https://github.com/muesli/duf)

A better `df` alternative.

![duf](https://raw.githubusercontent.com/muesli/duf/master/duf.png)


#### Installation

```zsh
brew install dust
```

#### Configuration

```zsh
alias df='duf'
```

## [broot](https://github.com/Canop/broot)

A new way to see and navigate directory trees.

![broot](https://raw.githubusercontent.com/Canop/broot/main/website/docs/img/20230129-overview.png)


#### Installation

```zsh
brew install broot
```

#### Configuration

```zsh
broot
```

## [fd](https://github.com/sharkdp/fd)

A simple, fast and user-friendly alternative to `find`.

![fd](https://raw.githubusercontent.com/sharkdp/fd/9ce43b2d7b1ae80c53e8801d2ce4c0499e88d78f/doc/screencast.svg)


#### Installation

```zsh
brew install fd
```

## [ripgrep](https://github.com/BurntSushi/ripgrep)

An extremely fast alternative to `grep` that respects your gitignore.

![ripgrep](https://user-images.githubusercontent.com/200613/90223748-ecaeab80-de0e-11ea-9140-ac9219f5747c.gif)


#### Installation

```zsh
brew install ripgrep
```

## [mcfly](https://github.com/cantino/mcfly)


Fly through your shell `history`. 

![mcfly](https://raw.githubusercontent.com/cantino/mcfly/master/docs/screenshot.png)

#### Installation

```zsh
brew tap cantino/mcfly
brew install cantino/mcfly/mcfly
```

#### Configuration

```zsh
eval "$(mcfly init zsh)"
```

## [as-tree](https://github.com/jez/as-tree)

Print a list of paths as a tree of paths.

For example, given:
```
dir1/foo.txt
dir1/bar.txt
dir2/qux.txt
```

it will print:
```
.
├── dir1
│   ├── foo.txt
│   └── bar.txt
└── dir2
    └── qux.txt
```

#### Installation

```zsh
brew install as-tree
```

## [jq](https://github.com/jqlang/jq)

The `sed` for JSON data. 

![jq](https://camo.githubusercontent.com/493aad4897e0effc0224c8e30a6c8fde99448988e6d09af8e10fee1a8420aa85/68747470733a2f2f626c6f672e6e6f656e6965746f2e636f6d2f6d656469612f676e6f6d652d7368656c6c2d73637265656e73686f742d564d4142555a2e706e67)

#### Installation

```zsh
brew install jq
```

## [fq](https://github.com/wader/fq)

Tool, language and decoders for working with binary data.

![fq](https://raw.githubusercontent.com/wader/fq/dea9303bbe267987486f4b5785ae4ac11c7d3b10/doc/demo.svg)

#### Installation

```zsh
brew install fq
```

## [cheat](https://github.com/cheat/cheat)

Create and view interactive cheatsheets on the command-line.

![cheat](https://camo.githubusercontent.com/2a07dd2e9c5692208e78aae7071874191a84b6ca5edbcd2b2d33e7ca31804b1d/68747470733a2f2f7374617469632e68617964656e6a616d65732e696f2f77702d636f6e74656e742f75706c6f6164732f323032302f30392f63686561742d636f6d6d616e642d6c696e652d6769746875622d383638783437382e706e67)

#### Installation

```zsh
brew install cheat
```

## [tldr](https://github.com/tldr-pages/tldr)

A community effort to simplify `man` pages with practical examples.

![tldr](https://raw.githubusercontent.com/tldr-pages/tldr/6806784459325b56a5676374f1cd0e06979335e8/images/tldr.svg)

#### Installation

```zsh
brew install tldr
```

## [bottom](https://github.com/ClementTsang/bottom)

Yet another cross-platform graphical process/system monitor.

![bottom](https://raw.githubusercontent.com/ClementTsang/bottom/master/assets/demo.gif)

#### Installation

```zsh
brew install bottom
```

## [glances](https://github.com/nicolargo/glances)

Glances an Eye on your system. A top/htop alternative for GNU/Linux, BSD, Mac OS and Windows operating systems.

![glances](https://raw.githubusercontent.com/nicolargo/glances/develop/docs/_static/glances-summary.png)

#### Installation

```zsh
brew install glances
```

## [gping](https://github.com/orf/gping)

`ping`, but with a graph.

![gping](https://raw.githubusercontent.com/orf/gping/master/images/readme-example.gif)

#### Installation

```zsh
brew install gping
```

## [httpie](https://github.com/httpie/cli)

A modern, user-friendly command-line HTTP client for the API era.

![httpie](https://raw.githubusercontent.com/httpie/httpie/master/docs/httpie-animation.gif)

#### Installation

```zsh
brew install httpie
```

## [curlie](https://github.com/rs/curlie)

The power of `curl`, the ease of use of `httpie`.

![curlie](https://raw.githubusercontent.com/rs/curlie/master/doc/get.png)

#### Installation

```zsh
brew install curlie
```

## [dog](https://github.com/ogham/dog)

A user-friendly command-line DNS client. `dig` on steroids

![dog](https://raw.githubusercontent.com/ogham/dog/master/dog-screenshot.png)

#### Installation

```zsh
brew install dog
```

#### Configuration

```zsh
alias dig='dog'
```
