# docker-elasticsearch-cluster
docker-elasticsearch-cluster

## check
```
grep vm.max_map_count /etc/sysctl.conf
vm.max_map_count=262144
```

## set max_map_count
```
sysctl -w vm.max_map_count=262144
```

## permission
```
mkdir esdatadir
chmod g+rwx esdatadir
chgrp 0 esdatadir
```

## URL test running
```
http://localhost:9200/_cat/nodes?v=true&pretty
```
