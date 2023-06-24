ARG USERNAME=go
ARG USER_UID=1000
ARG USER_GID=$USER_UID

FROM golang:1.20.5

# Create the user
RUN groupadd --gid 1000 go \
    && useradd --uid 1000 --gid 1000 -m go

WORKDIR /home/go/app

USER go

CMD [ "tail", "-f", "/dev/null" ]