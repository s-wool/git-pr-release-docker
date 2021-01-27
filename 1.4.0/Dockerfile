FROM ruby:2.7-alpine

RUN  apk --update --no-cache add openssh git \
         && gem install -N git-pr-release:1.4.0 \
         && rm -rf /usr/local/lib/ruby/gems/2.5.0/cache/*.gem \
                   /usr/local/bundle/cache/*.gem

COPY ./entrypoint.sh /

ENTRYPOINT ["/entrypoint.sh"]