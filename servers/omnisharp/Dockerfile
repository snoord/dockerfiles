FROM debian:bullseye-slim

WORKDIR /tmp

RUN apt-get update \
  && apt-get install curl -y \
  && rm -rf /var/lib/apt/lists \
  && curl -L -O https://github.com/OmniSharp/omnisharp-roslyn/releases/download/v1.38.0/omnisharp-linux-x64.tar.gz \
  && tar -xf omnisharp-linux-x64.tar.gz -C /usr \
  && rm omnisharp-linux-x64.tar.gz

CMD [ "/usr/run", "--languageserver" ]
