redis-server redis-config/redis.conf - will start the redis server using the config file in ./redis-config
systemctl list-units --type=service | grep - redis will find a service with redis in the name
sudo systemctl stop redis-server.service - will stop the service

## redis benchmarks

redis-benchmark -t SET,GET -q
SET: 107296.14 requests per second, p50=0.383 msec
GET: 173310.22 requests per second, p50=0.143 msec
