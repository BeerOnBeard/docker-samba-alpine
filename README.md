# DO NOT EXPOSE TO THE INTERNET!

This container is wide open. It exposes a single share to anyone who can see this server on the network. Anyone can read/write files to this share. I'm using it to expose a share on a local network behind a firewall.

Example usage:
```bash
docker run -d \
  -p 137-139:137-139 \
  -p 445:445 \
  -v /host/path:/shared \
  beeronbeard/docker-samba-alpine;
```
