#
# Python Dockerfile + ssh for dockerbot
#
# https://github.com/dockerfile/python
#

# Pull base image.
FROM dockerfile/ubuntu

# Install Python, modules, clone git repo
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y python python-dev python-pip python-virtualenv
RUN pip install irc docker-py
RUN mkdir /src ; cd /src ; git clone https://github.com/dkoppel/dockerbot

# Define mountable directories.
VOLUME ['/src']

# Define working directory.
WORKDIR /src

# Define default command.
CMD ['/bin/bash']

