FROM debian:jessie

ADD apt/conf/99debversion /etc/apt/apt.conf.d/99debversion
# ADD apt/conf/99proxy /etc/apt/apt.conf.d/99proxy
ADD apt/sources.list /etc/apt/sources.list

# Update it all:
RUN apt-get update && \
    apt-get upgrade -y && \
    rm -rvf /var/lib/apt/lists/*

CMD ["/bin/bash"]
