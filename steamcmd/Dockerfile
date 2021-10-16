FROM amazonlinux:latest

WORKDIR /home

RUN yum update -y
RUN yum upgrade -y
RUN yum install -y glibc.i686
RUN yum install -y libstdc++.i686
RUN yum install -y tar
RUN yum install -y gzip
RUN yum install -y wget
RUN wget "https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz"
RUN tar xzvf ./steamcmd_linux.tar.gz
RUN mkdir ./cs_go
RUN ./steamcmd.sh
RUN login anonymous
RUN force_install_dir ./cs_go
# https://developer.valvesoftware.com/wiki/Dedicated_Servers_List , csgo=740
RUN app_update 740 validate
