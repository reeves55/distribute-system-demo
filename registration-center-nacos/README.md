#Nacos注册&配置中心

##直接单机模式启动

单机模式会把数据存储在本地,如果 ```application.properties``` 当中配置了db的地址等相关信息,则会使用指定的数据库,同时也会在本地derby数据库存储一份

```shell script
./nacos/bin/startup.sh -m standalone
```

##集群模式启动

###1. 配置cluster.conf

```text
10.10.109.214
11.16.128.34
11.16.128.36
```

###2. 配置application.properties
```text

```

###3. 启动Nacos集群

```shell script
./nacos/bin/startup.sh
```