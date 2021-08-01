# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.187.0/containers/alpine/.devcontainer/base.Dockerfile

# [Choice] Alpine version: 3.13, 3.12, 3.11, 3.10
ARG VARIANT="3.13"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-alpine-${VARIANT}

# ** [Optional] Uncomment this section to install additional packages. **
# RUN apk update \
#     && apk add --no-cache <your-package-list-here>
# Install python/pip
ENV PYTHONUNBUFFERED=1
RUN apk add --update --no-cache python3 && ln -sf python3 /usr/bin/python
RUN python3 -m ensurepip
RUN pip3 install --no-cache --upgrade pip setuptools