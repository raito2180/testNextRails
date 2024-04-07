FROM ruby:3.2.2

RUN apt-get update -qq && apt-get install -y nodejs postgresql-client

WORKDIR /back_end

COPY Gemfile Gemfile.lock /back_end/

RUN bundle install

COPY . /back_end/