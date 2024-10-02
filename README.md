# uv_practice

## install
```
curl -LsSf https://astral.sh/uv/install.sh | sh


echo 'source $HOME/.cargo/env' >> ~/.zprofile
exec $SHELL -l

uv --version
```

## How to use
```
uv python list --all-versions
uv python list --all-platforms

uv python install 3.12

uv run --python 3.12 python -c 'print("hello world")'

```

## run script
```
uv run example.py
```

### Features
```
uv python install: Install Python versions.
uv python list: View available Python versions.
uv python find: Find an installed Python version.
uv python pin: Pin the current project to use a specific Python version.
uv python uninstall: Uninstall a Python version.
```


## Docs
https://docs.astral.sh/uv/