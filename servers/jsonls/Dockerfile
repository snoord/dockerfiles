FROM alpine:3.15.0

RUN apk add --no-cache \
  nodejs \
  npm \
  && npm install -g \
    vscode-json-languageserver

CMD [ "vscode-json-languageserver", "--stdio" ]
