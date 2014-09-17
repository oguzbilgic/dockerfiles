FROM ubuntu:12.04

# Install Haproxy.
RUN apt-get update
RUN apt-get install -y haproxy=1.4.18-0ubuntu1.2
RUN sed -i 's/^ENABLED=.*/ENABLED=1/' /etc/default/haproxy

# Add files.
ADD haproxy.cfg /etc/haproxy/haproxy.cfg
ADD start.bash /haproxy-start

# Define mountable directories.
VOLUME ["/haproxy-override"]

# Define working directory.
WORKDIR /etc/haproxy

# Define default command.
CMD ["bash", "/haproxy-start"]

# Expose ports.
EXPOSE 80
EXPOSE 443
EXPOSE 4001
