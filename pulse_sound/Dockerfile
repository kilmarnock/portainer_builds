FROM ubuntu:22.04

# Install package dependencies
RUN apt update -y && \
    DEBIAN_FRONTEND=noninteractive apt -qq install -y --no-install-recommends \
        python3-paho-mqtt \ 
        mpg321 \
        nano \
        libusb-1.0-0
        

RUN apt clean

ADD ./uhubctl /usr/bin
