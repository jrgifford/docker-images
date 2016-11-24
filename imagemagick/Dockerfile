FROM ubuntu:14.04.4
ENV DEBIAN_FRONTEND noninteractive
RUN \
  echo "deb http://archive.ubuntu.com/ubuntu trusty-backports main restricted universe multiverse" >> /etc/apt/sources.list

RUN \
  apt-get update && \
  apt-get -y install \
    povray && \
  rm -rf /var/lib/apt/lists/*

RUN \
  apt-get update && \
  apt-get -y install \
    software-properties-common && \
  apt-add-repository -y ppa:mc3man/trusty-media && \
  apt-get update && \
  apt-get -y install \
    ffmpeg && \
  rm -rf /var/lib/apt/lists/*

RUN \
  apt-get update && \
  apt-get -y install \
    ghostscript \
    libmagickcore5-extra \
    netpbm\
    autotrace\
    cups-bsd \
    curl \
    enscript \
    gimp \
    grads \
    groff-base\
    hp2xx \
    html2ps \
    libwmf-bin \
    mplayer \
    radiance \
    sane-utils \
    texlive-binaries \
    transfig \
    ufraw-batch \
    xdg-utils && \
  apt-get -y install \
    gnuplot \
    imagemagick-doc \
    imagemagick && \
  rm -rf /var/lib/apt/lists/*

RUN \
  apt-get clean

