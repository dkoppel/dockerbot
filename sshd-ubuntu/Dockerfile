# A quick little sshd dockerfile for dockerbot's shell function

FROM     ubuntu:14.04
RUN apt-get update && apt-get install -y openssh-server
RUN mkdir /var/run/sshd

# Set a root password here, or create additional accounts for SSH access.
RUN echo 'root:password' | chpasswd

# Permit root logins via SSHd conf.
RUN sed -i 's/PermitRootLogin without-password/PermitRootLogin yes/' /etc/ssh/sshd_config

EXPOSE 22
CMD ["/usr/sbin/sshd", "-D"]
