FROM ruby:3.2.1-bullseye

WORKDIR /tmp/docker_build

# Install jekyll.
RUN gem install jekyll bundler

# Change to the starting directory.
WORKDIR /workspace

# Cleanup once build is finished.
RUN rm -rf /tmp/docker_build
