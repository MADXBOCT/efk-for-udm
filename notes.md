# Setup steps
run `docker compose up -d`\
then
```bash 
docker cp efk-for-udm-es01-1:/usr/share/elasticsearch/config/certs/ca/ca.crt /tmp/. 
curl --cacert /tmp/ca.crt -u elastic:changeme https://localhost:9200
```
