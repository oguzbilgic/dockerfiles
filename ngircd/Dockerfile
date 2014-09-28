FROM ubuntu:14.04

RUN apt-get update
RUN apt-get install -y ngircd=21-1

EXPOSE :443
EXPOSE :6664
EXPOSE :6667

ENTRYPOINT ["/usr/sbin/ngircd"]
CMD ["-n"]
