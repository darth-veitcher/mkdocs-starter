# Introduction

This project is an example skeleton for a repository with documentation supported by [mkdocs](https://www.mkdocs.org) and published through GitHub Pages. It can be cloned and modified to kickstart off development, removing the need for time consuming configuration of good quality docs.

It supports the following:

* Publishing with Github Pages (using `master` branch and `/docs`)
* Mkdocs material theme
* Dark/Light mode
* Customised theme
* Embedding of interactive draw.io diagrams
* Built in search across the documentation

## Getting Started

### Installation

Simply clone the repository and then overwrite with your own.

```zsh
# clone
git clone git@github.com:darth-veitcher/mkdocs-starter.git new-project
```

```zsh
# overwrite and initialise a new empty one
cd new-project
rm -rf .git/
git init .
```

### Usage

To build and launch the documentation the requirements have been configured as development dependencies. Install these with `pipenv install --dev`.

Build the documentation with `pipenv run mkdocs build` or view a preview of the documentation with `pipenv run mkdocs serve`.

The output from the `build` process is a html website in the `/docs` folder whereas a `serve` command runs a local webserver available at [http://127.0.0.1:8000](http://127.0.0.1:8000) for viewing of the documentation.

### Dependencies

* Python 3
* Pipenv (can be installed with `pip`)

The project ships with a `Pipfile` for use with [pipenv](https://pipenv.pypa.io/en/latest/). Depending on your shell configuration this may automatically be detected and configured for you, otherwise please install the `--dev` requirements.

## Contribute

Pull requests and contributions are welcome. This is designed to be a fairly minimal starter project.
