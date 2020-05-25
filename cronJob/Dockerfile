FROM alpine:3.11.6
LABEL maintainer="Sergii Kotenko"
LABEL version="0.1"

# ADD curl PACKAGE
RUN apk update --no-cache && apk add --no-cache curl=7.67.0-r0

# Remove dependencies
RUN rm -fr /var/cache/apk/*
