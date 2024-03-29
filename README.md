# Python Starter Repo

All information and shortcuts for Python Language.

## Table of contents

- [Python Starter Repo](#python-starter-repo)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
  - [Install](#install)
  - [Set up new python env](#set-up-new-python-env)
  - [Set up Environments with Anaconda](#set-up-environments-with-anaconda)
    - [Conda Commands](#conda-commands)
    - [Using with VS code](#using-with-vs-code)
  - [Set up cmd commands](#set-up-cmd-commands)
    - [Aditional parts](#aditional-parts)
  - [Environments](#environments)
  - [Modules](#modules)
    - [My Laptop location](#my-laptop-location)
  - [General](#general)
  - [Project dependencies](#project-dependencies)
    - [Commands](#commands)
    - [Data notes](#data-notes)
    - [Extensions (VSCode)](#extensions-vscode)

## Overview

On windows use CMD to execute commands.

Python is a great language for AI and machine learning.

## Install

1. Create file to store python and download and install `mkdir pyver`
2. Use custom install on python - comes with pip
   1. Do not add PATH
   2. Tick install for all users
   3. set install location to created directory plus `/py<versionNumber>`

## Set up new python env

1. Open CMD adn locatie python directory``
2. Create project directory
3. install the environment `python -m venv projectName`
4. Directory projectName will be created
5. `<projectName>\Scripts\activate` activate the environment
6. `pip install numpy` add modules
7. `pip list` see all packages
8. Create a main.py file using vscode and add

```py
import random

# Generate a random number between 1 and 10
random_number = random.randint(1, 10)

print(f"Random number: {random_number}")
```

8. From cmd run `python <projectname>/main.py` to run in command line.


## Set up Environments with Anaconda

1. Open cmd
2. Run `conda` to check install
3. To create run `conda create --name <nameEnv> python=3.11`
4. `conda list` see all packages

### Conda Commands

`conda info --envs` see all environments
`conda list` see all packages
`conda env remove -n <envName>` remove env

### Using with VS code



## Set up cmd commands

1. Create a file `type nul > script.py`
2. `echo var1 = 10 >> script.py` add code
3. Install all dependencies from txt file `pip install -r requirements.txt`
4. `pip install <package-name> --user` packages error free

### Aditional parts

1. Python shell
2. PIP - get modules from online packages

## Environments

Environments are a sandbox where you can install packages and test code.

## Modules

1. `import time` This is the time and date modules
2. `import calendar` Calander

### My Laptop location

- `c:/Users/Tom/pyver/py311/python -m venv abctest` create new environment inside empty directory

## General

- `python` command is shorthand for the file location
- cntr shift p - set interpreter

## Project dependencies

- numpy - math module `pip install numpy`

### Commands

pip

- `pip list --outdated --format=freeze | grep -v '^\-e' | cut -d = -f 1  | xargs -n1 pip install -U` update all
- `pip list --outdated --format=freeze | findstr -v '^\-e' | cut -d = -f 1  | xargs -n1 pip install -U` update all
- `pip freeze --local | Select-String -v '^\-e' | cut -d = -f 1 | xargs -n1 pip install -U` ## cmd update
- `pip install "psycopg[binary]"` for server sql
- `pip install "psycopg[pool]"`

flask

- `pip install flask`
- `pip install flask-login`
- `pip install flask-sqlalchemy`

django

- `python -m pip install Django` in active env
- `django-admin startproject mysite` install package
- `python manage.py runserver` run server
- `python manage.py runserver 8080` run on port 8080
- `mython manage.py startapp main`
- `python manage.py migrate` compile new files added
- `python manage.py makemigrations <NAME>` add new fields to database
- `python manage.py migrate` compile new files added (AGAIN)

### Data notes

- file modes 'w (write)', 'r (read)', 'a (append)'
- a will write to the end of the file or create a new file
- `__init__.py` makes website folder a package

### Extensions (VSCode)

- jinja - html python injection script
