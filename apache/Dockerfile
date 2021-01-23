# MyUnraid - ENJOY IT
# Use a temporary image to compile and test the libraries
FROM nextcloud:production-apache

# Upgrade and update
RUN apt upgrade && apt -y update

RUN set -ex; \
    \
    apt-get update; \
    apt-get install -y --no-install-recommends \
        ffmpeg \
        imagemagick \
        ghostscript \
    ; \
    rm -rf /var/lib/apt/lists/*
    
    ENV NEXTCLOUD_UPDATE=1
