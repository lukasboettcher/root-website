# to run
docker run -d --restart unless-stopped --name root-website -l traefik.enable=true \
    -l traefik.http.routers.root.rule="Host(\`<HOST>\`)" -l traefik.http.routers.root.entrypoints=websecure \
    -l traefik.http.routers.root.tls.certresolver=letsencrypt ghcr.io/lukasboettcher/root-website:master