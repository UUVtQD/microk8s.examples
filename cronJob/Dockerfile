FROM alpine:3.11.6
LABEL maintainer="Sergii Kotenko"
LABEL version="0.1"

# ADD curl PACKAGE
RUN apk update --no-cache && apk upgrade --no-cache && apk add --no-cache curl

# Remove dependencies
RUN rm -fr /var/cache/apk/*