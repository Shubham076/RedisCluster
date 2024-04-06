Go into each folder and 

redis-server redis7000.conf
redis-server redis7001.conf
redis-server redis7002.conf

redis-cli --cluster create 127.0.0.1:7000 127.0.0.1:7001 127.0.0.1:7002 --cluster-replicas 0

redis-cli -c -p 7000 // to test local client
