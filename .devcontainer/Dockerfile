FROM ruby:2.7.4-bullseye

# Change to the starting directory.
WORKDIR /workspace
RUN mkdir docs
RUN cd docs

# Install jekyll and bundler.
RUN gem update --system
RUN gem install bundler
RUN gem install jekyll

