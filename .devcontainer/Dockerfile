FROM ruby:3.3.0-slim-bullseye

# ARG USERNAME=vscode
# ARG USER_UID=1000
# ARG USER_GID=$USER_UID

# RUN apt-get update \
#     && groupadd --gid $USER_GID $USERNAME \
#     && useradd -s /bin/bash --uid $USER_UID --gid $USER_GID -m $USERNAME \
#     && apt-get install -y sudo \
#     && echo $USERNAME ALL=\(root\) NOPASSWD:ALL > /etc/sudoers.d/$USERNAME \
#     && chmod 0440 /etc/sudoers.d/$USERNAME

RUN apt-get update && apt-get -y install build-essential zlib1g-dev

RUN gem install jekyll bundler jekyll-compose

WORKDIR /workspace

EXPOSE 4000