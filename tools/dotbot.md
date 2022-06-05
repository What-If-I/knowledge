tags: #python #package-manager 
# A tool that bootstraps your dotfiles ⚡️
Dotbot makes installing your dotfiles as easy as `git clone $url && cd dotfiles && ./install`, even on a freshly installed system!

Dotbot is a tool that bootstraps your dotfiles (it's a [Dot]files [bo]o[t]strapper, get it?). It does _less_ than you think, because version control systems do more than you think.

Dotbot is designed to be lightweight and self-contained, with no external dependencies and no installation required. Dotbot can also be a drop-in replacement for any other tool you were using to manage your dotfiles, and Dotbot is VCS-agnostic -- it doesn't make any attempt to manage your dotfiles.

See [this blog post](https://www.anishathalye.com/2014/08/03/managing-your-dotfiles/) or more resources on the [tutorials page](https://github.com/anishathalye/dotbot/wiki/Tutorials) for more detailed explanations of how to organize your dotfiles.

## Install
## Init
```bash
cd ~/.dotfiles # replace with the path to your dotfiles
git init # initialize repository if needed
git submodule add https://github.com/anishathalye/dotbot
git config -f .gitmodules submodule.dotbot.ignore dirty # ignore dirty commits in the submodule
cp dotbot/tools/git-submodule/install .
touch install.conf.yaml
```
### On macOS ([[pipx]])
```bash
pipx install dotbot
```

## Usage
There a lot to read. Better refer to original [documentation](https://github.com/anishathalye/dotbot#full-example).
## Links
**Documentation**: [github](https://github.com/anishathalye/dotbot)