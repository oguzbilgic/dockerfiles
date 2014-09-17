## haproxy

### Run

```bash
docker run -d -p 80:80 443:443 4001:4001 --link <app-host>:app oguzbilgic/haproxy
```
