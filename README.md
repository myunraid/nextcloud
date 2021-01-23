# Nextcloud on Docker with: ffmpeg imagemagick ghostscript
This Dockerfile extends the official nextcloud:apache Dockerfile (https://hub.docker.com/_/nextcloud) with preview apps in your Nextcloud images.

# Installation
In general, follow the instructions on https://hub.docker.com/_/nextcloud to use this image. Especially please check out the environment variables to configure your nextcloud docker installation.

# Post installation configuration
I recommend activate the cron scheduler, which is part of the image. Go to Settings -> Basic Settings and select the option "Cron" for the Background jobs. That's make the web interface more responsive, especially with a lot of files or if you have many users. Background jobs are executed every 5 minutes.
