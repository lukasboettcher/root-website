# to run
docker run -d --restart unless-stopped -e "LETSENCRYPT_HOST=btchr.de" -e "VIRTUAL_HOST=btchr.de" -v /var/www:/var/www --name btchr-root-website btchr-root-website
