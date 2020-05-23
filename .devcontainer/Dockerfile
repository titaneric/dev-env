FROM rust:1

WORKDIR /home/workspace

RUN apt-get update

RUN apt-get install -y git openssh-client

RUN apt-get install -y zsh

RUN sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

RUN rustup update 2>&1

RUN cargo install exa fd-find ripgrep

CMD ["zsh"]