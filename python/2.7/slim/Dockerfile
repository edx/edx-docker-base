# docker build -t edxops/python:2.7 - < python/2.7/slim/Dockerfile

FROM python:2.7-slim
ENV PYTHONUNBUFFERED 1

RUN apt-get update && \
    apt-get install --no-install-recommends -y curl && \
    curl -sL https://deb.nodesource.com/setup_6.x | bash - && \
    curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add - && \
    echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list && \
    apt-get update && \
    apt-get install --no-install-recommends -y \
        build-essential \
        gettext \
        git \
        libffi-dev \
        libjpeg-dev \
        libmemcached-dev \
        libmysqlclient-dev \
        libpng12-dev \
        libssl-dev \
        nodejs \
        yarn \
    && rm -rf /var/lib/apt/lists/*

## See https://github.com/krallin/tini/releases for latest release number
ARG TINI_VERSION=v0.14.0
ADD https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini /tini
RUN chmod +x /tini
ENTRYPOINT ["/tini", "--"]
