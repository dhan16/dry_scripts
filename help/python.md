## MacOS
  1. brew install python python3

## Python2.7
### virtualenv
  1. pip install virtualenv
  2. virtualenv <name> -p python2; deactivate

### spyder
    Use Anaconda

## Python3
### venv
    python3 -m venv /path/to/new/virtual/environment
    source /path/to/new/virtual/environment/bin/activate
    deactivate

### spyder
    1. pip install -U spyder
    2. pip install pyqt5

### push to PyPI
    https://packaging.python.org/tutorials/packaging-projects/
#### Setup
    1. python3 -m pip install --user --upgrade setuptools wheel twine
#### Push
    1. Change version in setup.py
    2. python3 setup.py sdist bdist_wheel
    3. twine upload dist/*