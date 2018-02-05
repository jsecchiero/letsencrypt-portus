
# Letsencrypt Portus

Deploy portus with auto-generated ssl certificate with letsencrypt. 
Using the idea of thpham/portus-registry-tls-compose.

# Usage

edit each .env variable before deploy

PORTUS_FQDN and REGISTRY_FQDN must be reachable domain from internet to work

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
