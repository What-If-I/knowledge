tags: #zsh #bash #plugin-manager
# The plugin manager for zsh.
Antigen is a small set of functions that help you easily manage your shell (zsh) plugins, called bundles. The concept is pretty much the same as bundles in a typical vim+pathogen setup. Antigen is to zsh, what [Vundle](https://github.com/gmarik/vundle) is to vim.

## Install
```bash
curl -L git.io/antigen > antigen.zsh
# or use git.io/antigen-nightly for the latest version
```
### On MacOS ([[brew]])
```bash
brew install antigen
```
## Usage
The usage should be very familiar to you if you use Vundle. A typical `.zshrc` might look like this:
```
source /path-to-antigen/antigen.zsh

# Load the oh-my-zsh's library.
antigen use oh-my-zsh

# Bundles from the default repo (robbyrussell's oh-my-zsh).
antigen bundle git
antigen bundle heroku
antigen bundle pip
antigen bundle lein
antigen bundle command-not-found

# Syntax highlighting bundle.
antigen bundle zsh-users/zsh-syntax-highlighting

# Load the theme.
antigen theme robbyrussell

# Tell Antigen that you're done.
antigen apply
```

Open your zsh with this `.zshrc` and you should see all the bundles you defined here, getting installed. Once it's done, you are ready to roll. The complete syntax for the `antigen bundle` command is discussed in the [Commands](https://github.com/zsh-users/antigen/wiki/Commands) page.

Furthermore, [In the wild](https://github.com/zsh-users/antigen/wiki/In-the-wild) wiki section has more configuration examples. You may as well take a look at the [Show off](https://github.com/zsh-users/antigen/wiki/Show-off) wiki page for interactive mode usage.

## Links
**Documentation**: [github](https://github.com/zsh-users/antigen)