FROM biocontainers/biocontainers:vdebian-buster-backports_cv1
MAINTAINER biocontainers <biodocker@gmail.com>
LABEL    software="biomaj3-core" \ 
    base_image="biocontainers/biocontainers:vdebian-buster-backports_cv1" \ 
    container="biomaj3-core" \ 
    about.summary="BioMAJ core library - Python 3.X" \ 
    about.home="https://github.com/genouest/biomaj-core" \ 
    software.version="3.0.15-1-deb-py3" \ 
    upstream.version="3.0.15" \ 
    version="1" \ 
    about.copyright="Olivier Sallou <olivier.sallou@irisa.fr>" \ 
    about.license="AGPL-3" \ 
    about.license_file="/usr/share/doc/biomaj3-core/copyright" \ 
    about.tags=""

USER root
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && (apt-get install -t buster-backports -y python3-biomaj3-core || apt-get install -y python3-biomaj3-core) && apt-get clean && apt-get purge && rm -rf /var/lib/apt/lists/* /tmp/*
USER biodocker
