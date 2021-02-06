# C extension for Python

This project implements a wrapper for c function fput to write an string to a file
In other words, this is c extension for python. 

## Setting up the project
```bash
python -m venv venv
source ./venv/bin/activate

# go to source directory of this project
# and execute setup.py to install the module
python setup.py install

# you can choose gcc or clang for compilation like below
CC=clang python setup.py install
CC=gcc python setup.py install
```

# Executing the c extension from python
```bash
# import our module to python
>>> import fputs

# execute out function
>>> fputs.fputs("Hello World!", "./dummy_text.txt")
```

## Reference
1. https://realpython.com/build-python-c-extension-module/