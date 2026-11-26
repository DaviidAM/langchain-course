FROM mcr.microsoft.com/devcontainers/python:1-3.12-bookworm

# The base image's Yarn apt repo has an expired GPG key, which breaks apt-get update in features.
RUN rm -f /etc/apt/sources.list.d/yarn.list

COPY --from=ghcr.io/astral-sh/uv:latest /uv /uvx /usr/local/bin/
