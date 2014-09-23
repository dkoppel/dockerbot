#
# Python Dockerfile + ssh for dockerbot
#
# https://github.com/dockerfile/python
#

# Pull base image.
FROM dockerfile/ubuntu

# Install Python, modules, clone git repo
RUN apt-get install -y python python-dev python-pip python-virtualenv
RUN pip install irc docker-py
RUN cd data ; git clone http://github.com/kuroishi/dockerbot 

# Define mountable directories.
VOLUME ['/data']

# Define working directory.
WORKDIR /data

# Define default command.
CMD ['/bin/bash']

