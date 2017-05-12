# docker build -t edxops/python:3.5 - < python/3.5/slim/Dockerfile

FROM python:3.5-slim
ENV PYTHONUNBUFFERED 1

RUN apt-get update && \
    apt-get install --no-install-recommends -y curl && \
    curl -sL https://deb.nodesource.com/setup_6.x | bash - && \
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
    && rm -rf /var/lib/apt/lists/*
