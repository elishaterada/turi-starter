# Turi Create on macOS

- [Turi Create](https://github.com/apple/turicreate)
- [Jupyter Notebook](https://jupyter.org/)


# System Requirements

- macOS version 10.12+


# Setup

The latest version of Turi Create does not support Python 3.7.x so you’ll need to install 3.6.x in your environment.

Turi Create takes advantage of host OS (macOS) so containerization is not the ideal solution for speed.

Install following tools to isolate your host development environment from project specific environment.

- `xcode-select --install` (to resolve zlib not available issue)
- Install Python 3.6.8 with [pyenv](https://github.com/pyenv/pyenv)
- Install [virtualenv](https://virtualenv.pypa.io/en/stable/installation/)
- Install [direnv](https://direnv.net/)


## Troubleshooting `zlib not available`

- Try `xcode-select --install`
- Try `CFLAGS="-I$(xcrun --show-sdk-path)/usr/include" pyenv install 3.6.8`


## Resources on using above tools together

- [Awesomely easy virtualenvs on OSX using pyenv and direnv](https://gist.github.com/alexhayes/cb1e6ad873c147502132ae17362a9daf)
- [Virtualenv + direnv setup script](https://github.com/elishaterada/venv-python)


# Install dependencies

```
cd /path/to/repo
pip install -r requirements.txt
```

# Start Jupyter Notebook

```
jupyter notebook
```
