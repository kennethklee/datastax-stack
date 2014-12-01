datastax-stack
==============

Simple single node datastax stack


Analytics Mode
--------------

Edit `/etc/default/dse`. Set `HADOOP_ENABLED=1`.


Cassandra Listening Port
------------------------

Edit `/etc/dse/cassandra/cassandra.yaml`. Set `rpc_port = 0.0.0.0`.


Starting DataStax
-----------------

```bash
sudo service dse start
sudo service datastax-agent start
sudo service opscenterd start
```

Browse to `http://10.0.0.3:8888` then click Existing Cluster. The ip is `localhost`.


Using Hive
----------

`dse hive`
