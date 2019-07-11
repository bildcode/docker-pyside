FROM python:2.7-slim-stretch

RUN apt-get update && \
    apt-get autoclean && \
    apt-get install -y libqt4-dev cmake xvfb && \
    rm -rf /var/cache/apk/* && \

    python -m pip install --no-cache-dir --upgrade pip && \
    pip install --no-cache-dir pyside && \
    pip install --no-cache-dir Qt.py && \
    pip install --no-cache-dir pytest pytest-cov anybadge pylint devpi-client

CMD ["bin/bash"]

apk update && apk upgrade && \
    apk add --update alpine-sdk nano qt5-qtbase qt5-qttools-dev && \
    rm -rf /var/cache/apk/*

