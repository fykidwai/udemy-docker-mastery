FROM ubuntu:latest
RUN apt-get update && apt-get -y install apache2-utils && rm -rf /var/lib/apt/lists/*
ENTRYPOINT [ "ab" ]
CMD ["--help"]