
# PyNation

[![PyPI Version](https://img.shields.io/pypi/v/pynation)](https://pypi.org/project/pynation)
![GitHub](https://img.shields.io/github/license/mrbazzan/pynation)
[![PyPI Publish](https://github.com/mrbazzan/pynation/actions/workflows/b_python-publish.yml/badge.svg?branch=v0.2)](https://github.com/mrbazzan/pynation/actions/workflows/b_python-publish.yml)
[![Tests](https://github.com/mrbazzan/pynation/actions/workflows/a_run-test.yml/badge.svg?branch=main)](https://github.com/mrbazzan/pynation/actions/workflows/a_run-test.yml)

Get information about a country. ``pynation`` is a command line application that helps users get quick information about a country.

Sometimes, people need quick info about a country, this application provides information like Alpha-2 code, currency, states in a country et.c.</p>

## INSTALL
PyNation requires Python 3.7 and above

MacOS / Linux:

```shell
$ python3 -m pip install pynation
```

Windows:

```cmd
> python -m pip install pynation
```


## Using the CLI application

The CLI can be invoked with the `pynation` command.

To get the help page:

```shell script
> pynation --help
```
![Example](/assets/help.gif)


```shell script
> pynation `countryname`
> pynation info `countryname`
```
![Example](/assets/info.gif)


```shell script
> pynation short `countryname`
> pynation short `countryname` -ab=3
```
![Example](/assets/short.gif) ![Example](/assets/long.gif)


## Hacking

If you want to edit the source code:
- Clone the repository

- Create a virtual environment
```        
    python3 -m venv venv/
```

- Activate the virtual environment
  - For Linux
    ```
    source venv/bin/activate
    ```
  - For Windows CMD
  ```
  cd venv/Scripts
  activate
  ```

- Upgrade the Pip version <**very important**>
```        
    pip install -U pip
```

- Install the package in editable mode `-e/--editable`
with the "dev" extra included
```        
    pip install -e '.[dev]'
```

This installs `pynation` from the source directory and changes
will be immediately reflected. It also installs extra development tools such as `pytest`


## Feedback

If you find a bug, please [file an issue](https://github.com/mrbazzan/pynation/issues).

If you have feature requests, please [file an issue](https://github.com/mrbazzan/pynation/issues)
and use the appropriate label

## How to Contribute

Please **raise an issue** before making a PR, so that the issue and implementation can be discussed before you write any code. **This will save you time**, and increase the chances of your PR being merged without significant changes. 

Please make PR's on a **new branch**, and _not_ on main. 

Please **include tests** for any PR's that include code (unless current tests cover your code contribution).

## Source of data

PyNation's data is scraped from the web, and the scrapers are stored at [url](https://github.com/mrbazzan/populate_pynation).
