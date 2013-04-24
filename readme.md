# Homebrew
``` sh
ruby -e "$(curl -fsSL https://raw.github.com/mxcl/homebrew/go)"
```
# Rbenv
~~~ sh
$ brew update
$ brew install rbenv
$ brew install ruby-build
~~~

# Vim

On Mac Os X installing MacVim updates vim terminal version

```bash
$ brew install macvim
```

# Janus

Janus is a distribution of plug-ins and mappings for Vim, Gvim and
MacVim.

To install it run the following command:

```bash
$ curl -Lo- https://bit.ly/janus-bootstrap | bash
```

Janus requires `ack`, `ctags` utilities, install them with the following commands:

```bash
$ brew install ack
```
and
```bash
$ brew install ctags
```

# Clone the repo including submodules
```bash
git clone --recursive git://github.com/bncoelho/dotfiles.git 
```

# Vim Powerline font

Change your terminal font to use one of the patched fonts and then run
the :PowerlineClearCache command inside vim
