# Dockerbot #

## About ##
This project is a fun way for me to familiarize myself with CoreOS and Docker.  I'm making an IRC bot to provision and manage containers on a CoreOS system.

This project was inspired by PumpingStationOne and it's members, and is intended for use in the #pumpingstationone channel on freenode.  Support your local hackerspace or makerspace.

## Requirements ##
* A Docker-ready server environment (This project was written and intended with CoreOS in mind for this environment, but any Docker daemon configured to listen on a tcp port will do.) - http://coreos.com - http://docker.io
* irc - https://pypi.python.org/pypi/irc
* docker-py - https://github.com/docker/docker-py

## Get Started ##
` $ dockerbot irc.someserver.net coreos-docker-api:2375 \#dockerbot dockerbot`
