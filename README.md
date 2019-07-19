# Debian, Python 2.7, Qt4, PySide + CI helpers
Built off of the official [`python:2.7-slim-stretch`](https://hub.docker.com/_/python) images, which are based on Debian. 

The intention is to have lightweight containers that work well with CI runners.
We start in a bash shell, so we can 
conveniently configure our CI setup from here.

# Dockerfiles / Tags
The containers are automatically updated when their base images do.
* latest (based on python:2.7-slim-stretch)
* develop (from my develop branch, experimental)

# Pre-installed pip packages
* anybadge
* devpi-client
* flake8
* pylint
* pyside
* pytest==4.6.4  (latest working for py2.7)
* pytest-cov
* pytest-qt
* pytest-xvfb
* Qt.py
* xvfbwrapper
