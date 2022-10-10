FROM thomasweise/docker-texlive-thin

# Install wget
RUN apt-get -y update
RUN apt-get install wget

COPY ./docker/local/resume/fonts /usr/local/share/fonts

# Install Zsh
RUN sh -c "$(wget -O- https://github.com/deluan/zsh-in-docker/releases/download/v1.1.2/zsh-in-docker.sh)"
