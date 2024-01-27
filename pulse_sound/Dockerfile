FROM ubuntu:22.04

# Install package dependencies
RUN apt update -y && \
    DEBIAN_FRONTEND=noninteractive apt -qq install -y --no-install-recommends \
        mpg321 \
        nano \
        libusb-1.0-0 \
        python3-paho-mqtt

RUN apt clean

ADD ./uhubctl /usr/bin
