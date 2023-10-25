# python

## Install python

- Use [`pyenv`](https://github.com/pyenv/pyenv) for python versions

```bash
# install
brew update
brew install pyenv
# shell for .zshrc
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
echo 'command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(pyenv init -)"' >> ~/.zshrc
```

## VSCode Extensions

- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- [Black Formatter](https://marketplace.visualstudio.com/items?itemName=ms-python.black-formatter)

## Django

[django](https://www.djangoproject.com/)

```bash
python -m pip install Django
```
