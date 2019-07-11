FROM python:2.7-slim-stretch

RUN apt-get update && \
    apt-get autoclean && \
    apt-get install -y --no-install-recommends libqt4-dev cmake build-essential xvfb && \
    rm -rf /var/cache/apk/* && \

    python -m pip install --no-cache-dir --upgrade pip && \
    pip install --no-cache-dir pyside && \
    pip install --no-cache-dir Qt.py && \
    pip install --no-cache-dir pytest==4.6.4 pytest-cov anybadge pylint devpi-client && \

    apt-get purge -y build-essentials && \
    apt-get purge -y cmake

CMD ["bin/bash"]
