# Debian, Python 2.7, Qt4, PySide + CI helpers
Built off of the official [`python:2.7-slim-stretch`](https://hub.docker.com/_/python) images, which are based on Debian. 

The intention is to have lightweight containers that work well with CI runners like the ones in GitLab.
We start in a bash shell on purpose, so we can 
conveniently configure our CI setup from here.

# Dockerfiles / Tags
The containers are automatically updated when their base images do.
* latest (based on python:2.7-slim-stretch)
* develop (from my develop branch, experimental)

# Pre-installed pip packages
* PySide2
* Qt.py
* pytest
* pytest-cov
* pylint
* devpi-client
* anybadge
