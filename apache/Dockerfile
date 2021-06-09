# https://myunraid.ru/ - ENJOY IT
# Use a temporary image to compile and test the libraries
FROM nextcloud:production-apache as builder

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
ENV PHP_MEMORY_LIMIT=1G
