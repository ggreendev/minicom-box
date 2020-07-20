############################################################
# Dockerfile to build minicom  container images
# Based on Alpine linux
############################################################

# Set the base image to alpine
FROM arm32v7/alpine:latest

# File Author / Maintainer
MAINTAINER Garrett Green

# Update the repository sources list
RUN apk update  && \ 
apk add minicom && \
rm -rf /tmp/src && \
rm -rf /var/cache/apk/*  

ENV device=/dev/mydevice 
ENV baud=115200 

CMD  minicom -D $device -b $baud 
