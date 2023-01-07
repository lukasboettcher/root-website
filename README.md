# to run
docker run -d --restart unless-stopped --name root-website \
    -l traefik.http.routers.root.rule="Host(\`<HOST>\`)" \
    ghcr.io/lukasboettcher/root-website:master