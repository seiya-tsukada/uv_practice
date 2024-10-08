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

## How to use venv
```
cd [path]/[to]/[dir]
uv venv # uv venv [dir]
source ./.venv/bin/activate

uv pip freeze
uv pip install flask
```

### transition venv
```
uv pip freeze | uv pip compile - -o requirements.txt


uv pip sync requirements.txt
```

### How to deactivate
```
deactivate
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