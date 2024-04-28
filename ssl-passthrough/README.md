
```sh

sudo docker build -t nginx-ssl-passthrough:v1 . --load
docker run -d --name nginx-ssl-proxy -p 443:443 nginx-ssl-passthrough:v1
openssl s_client -connect localhost:443 -servername example.mydomain.com

```