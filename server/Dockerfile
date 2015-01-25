#
# Python Dockerfile for dockerbot
#
# Based on https://github.com/dockerfile/python
#

# Pull base image.
FROM dockerfile/ubuntu

# Install Python, modules, clone git repo
RUN pip install irc docker-py GitPython
RUN mkdir /src ; cd /src ; git clone https://github.com/dkoppel/dockerbot

# Define mountable directories.
VOLUME ['/src']

# Define working directory.
WORKDIR /src

# Define default command.
CMD ['/bin/bash']

