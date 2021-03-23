FROM ubuntu:20.04

ENV MATTERMOST_VERSION=5.22.4

RUN apt-get update && apt-get install -y curl

RUN curl -sSL https://github.com/mattermost/mattermost-push-proxy/releases/download/v${MATTERMOST_VERSION}/mattermost-push-proxy.tar.gz | tar -xz

EXPOSE 8066
ENTRYPOINT ["/mattermost-push-proxy/bin/mattermost-push-proxy"]
