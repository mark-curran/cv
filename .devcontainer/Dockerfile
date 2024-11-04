FROM ruby:3.2.6-bullseye
ARG JEKYLL_VERSION

# Change to the starting directory.
WORKDIR /workspace
RUN mkdir docs

# Copy files we need to install dependencies
COPY docs/Gemfile /workspace/docs/Gemfile
COPY docs/Gemfile.lock /workspace/docs/Gemfile.lock

# Install jekyll and bundler.
WORKDIR /workspace/docs
RUN gem update --system
RUN gem install bundler
RUN gem install jekyll --version $JEKYLL_VERSION
RUN bundle install