
# Letsencrypt Portus

using the idea of thpham/portus-registry-tls-compose with updated software.
Deploy portus with auto-generated ssl certificate with letsencrypt

# Usage

edit each .env variable before deploy

PORTUS_FQDN must be a reachable domain to work
REGISTRY_FQDN must be a reachable domain to work

deploy

```
docker-compose up -d
```

After the deploy go to portus.example.com:
- create a user
- edit _Name_ with `reigstry`
- edit _Hostname_ with `registry:5000`
- click on show advanced button
- edit _External Registry Name_ with `registry.example.com`
