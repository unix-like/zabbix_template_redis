# zabbix_template_redis

| item                        | trigger                             |
| :-------------------------: | :---------------------------------: |
| Blocked Clients             |                                     |
| Current Client Connections  |                                     |
| Current Connections Resived |                                     |
| Current Slave Connections   |                                     |
| Data Inbound                |                                     |
| Data Outbound               |                                     |
| Expired Keys                |                                     |
| Key Hit Rate                |                                     |
| Keyspace Hits               |                                     |
| Keyspace Misses             |                                     |
| Memory Out Keys             |                                     |
| Processed Commands          |                                     |
| ReadOnly                    |                                     |
| Redis is running            | Redis Server is Down on {HOST.NAME} |
| Replicate Offset(Master)    |                                     |
| Replicate Offset(Slave)     |                                     |
| Use memory                  |                                     |
| Use memory (by OS)          |                                     |
| Use memory Peak             |                                     |
| iops                        |                                     |

适用于zabbix3.4及以上版本,监控数据的采集也实现并行收集,此监控项目共包含2个文件:

1. userparameter_redis.conf
2. redis.xml

其中`userparameter_redis.conf`, 需要分发到各个redis服务器上，`redis.xml`作为模版文件导入zabbix中。

