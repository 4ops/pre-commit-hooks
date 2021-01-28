# Pre-commit hooks

Pre-commit hooks based on [pre-commit](https://pre-commit.com)

## Installation

### With pip

```console
$ pip install pre-commit
```

### With curl

```
$ curl https://pre-commit.com/install-local.py | python -
```

### More installation options

See pre-commit official [docs](https://pre-commit.com/#install)

## Usage

### Create pre-commit config file

Example content of `.pre-commit-config.yaml`
```yaml
repos:
  - repo: git://github.com/4ops/pre-commit-hooks
    rev: v1.1.0
    hooks:
        - id: terraform-fmt
        - id: packer-fmt
```

### Install hooks

```console
$ pre-commit install
```

### Manual run

```console
$ pre-commit run -a
```
