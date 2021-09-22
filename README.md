# ml-for-business

## setup virtual env
Get `brew install pyenv pyenv-virtualenv`

Then install python3.

See all available versions `pyenv install -l`

Install stable version 3 like `pyenv install 3.9.7`

Then create a virtual env giving it a name (py3 here)

`pyenv virtualenv 3.9.7 py3`

Add to .zshrc
```
eval "$(pyenv init -)"

export PATH="$(pyenv root)/shims:$PATH"
export PATH="$(pyenv root)/bin:$PATH"
```

Add to .zprofile 

```
eval "$(pyenv init --path)"
```
Above steps are all one-time.

Now create a new terminal. In the folder where you want to use py3:
`pyenv local py3`

Now everytime you enter that folder it will automatically switch to py3

Verify by:
```
$python -V 
$pyenv which python
```

Run `pip install -r requirements.txt` to install all required libraries.
