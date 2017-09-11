nginx-plex-deluge-proxy
=======================

This is an NGINX configuration to allow plex and all it's little helpers to stay behind a reverse proxy.

It gives you the following paths:

* `http://X.X.X.X/plex`
* `http://X.X.X.X/deluge`
* `http://X.X.X.X/radarr`
* `http://X.X.X.X/nzbget`
* `http://X.X.X.X/sonarr`
* `http://X.X.X.X/mylar`
* `http://X.X.X.X/headphones`
* `http://X.X.X.X/pyload`
* `http://X.X.X.X/jackett`
* `http://X.X.X.X/lazylibrarian`
* `http://X.X.X.X/nzbhydra`
* `http://X.X.X.X/ombi`
* `http://X.X.X.X/plexpy`

## Installation

### Step 1

Install Organizr (https://github.com/causefx/Organizr) and set the correct path in the media_proxy/sites-available.conf. And install and setup SSL-Certificats (https://certbot.eff.org).
In my case I had to block all the ports (except 80 and 443) with ufw...

### Step 2

These files need to be copied/cloned into the NGINX config folder, for example `/etc/nginx` on Ubuntu.

### Step 3

Restart NGNIX `sudo service nginx restart`

### Step 4

You should be able to open `http://X.X.X.X` and see Organizr now.
