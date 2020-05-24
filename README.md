# asdf-pipenv

[![githubactions](https://github.com/and-semakin/asdf-pipenv/workflows/build/badge.svg)](https://github.com/and-semakin/asdf-pipenv/actions)

[Pipenv](https://github.com/pypa/pipenv) plugin for [asdf](https://github.com/asdf-vm/asdf) version manager.
Inspired by [`asdf-poetry`](https://github.com/crflynn/asdf-poetry).

## Requirements

* `curl`;
* `python` (version 3.4 or newer).

## Limitations

At the moment, `pipenv` is installed by creating a virtual environment
using an active interpreter (system or installed via
[asdf-python](https://github.com/danhper/asdf-python)).
If the interpreter that was active at the time of installation
is subsequently deleted, the installed `pipenv` version will stop working.
To fix, you will have to reinstall affected `pipenv` version.

## Install

With [asdf](https://asdf-vm.com/) already installed:

```
asdf plugin-add pipenv https://github.com/and-semakin/asdf-pipenv.git
```

## Use

To list all versions

```bash
asdf list all pipenv
```

To install a specific version of `pipenv`:

```bash
asdf install pipenv 2018.11.26
asdf install pipenv 2020.4.1b2
```

To uninstall a specific version of `pipenv`:

```bash
asdf uninstall pipenv 2018.11.26
```

To set a global version of `pipenv`:

```bash
asdf global pipenv 2020.4.1b2
```

To set a project-specific version of `pipenv`:

```bash
asdf local pipenv 2018.11.26
```
