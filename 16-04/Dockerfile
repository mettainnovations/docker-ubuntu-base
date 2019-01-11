FROM ubuntu:16.04 AS ubuntu-base

# Install dependencies
RUN apt-get update -y && \
    apt-get install -y build-essential cmake cmake-curses-gui wget unzip git libavcodec-dev libavutil-dev libavutil-ffmpeg54 libavformat-dev libavfilter-dev libavdevice-dev libjpeg8-dev libpng16-dev libtiff5-dev libx264-dev libgstreamer1.0-dev libboost-all-dev && \
    apt-get install -y libopenblas-dev liblapack-dev qt5-default libqt5svg5-dev qtcreator libqt5serialport5-dev qtmultimedia5-dev && \
    apt-get clean -y

# Casa Blanca and DocumentDBCpp dependencies
RUN apt-get install -y libcpprest-dev libssl-dev uuid-dev

RUN mkdir -p /home/developer
ENV HOME /home/developer
WORKDIR /home/developer
