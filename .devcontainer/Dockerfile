FROM ruby:slim

RUN apt update \
    && apt install -y --no-install-recommends \
    apt-utils \
    git \
    build-essential \
    ca-certificates \
    procps \
    && apt autoremove -y \
    && apt clean -y \
    && rm -rf /var/lib/apt/lists/* \
    && gem install rubocop solargraph rubocop-performance rubocop-rails rubocop-packaging
