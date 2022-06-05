tags: #python #package-manager
# Install and Run Python Applications in Isolated Environments

pipx is a tool to help you install and run end-user applications written in Python. It's roughly similar to macOS's `brew`, JavaScript's [npx](https://medium.com/@maybekatz/introducing-npx-an-npm-package-runner-55f7d4bd282b), and Linux's `apt`.

It's closely related to pip. In fact, it uses pip, but is focused on installing and managing Python packages that can be run from the command line directly as applications.

## Install pipx
### On macOS ([[brew]])
```bash
brew install pipx
pipx ensurepath
```

Upgrade pipx with `brew update && brew upgrade pipx`.

### On Linux, install via pip (requires pip 19.0 or later)
```bash
python3 -m pip install --user pipx
python3 -m pipx ensurepath
```

Upgrade pipx with `python3 -m pip install --user -U pipx`.

## Usage
```bash
pipx install PACKAGE
```
## Links
**Documentation**: [https://pypa.github.io/pipx/](https://pypa.github.io/pipx/)
**Source Code**: [https://github.com/pypa/pipx](https://github.com/pypa/pipx)