# Overview

This interface is used in [layer-rethinkdb](https://github.com/tengu-team/layer-rethinkdb) for setting up a RethinkDB cluster.

#### Peers

```yaml
peers:
  cluster:
    interface: rethinkdb-cluster
```

```python
@when('cluster.connected')
def configure_cluster(cluster):
    units = cluster.get_peer_addresses()
    install_cluster(units)
```

# Contact Information

## Authors

 - Dixan Peña Peña <dixan.pena@tengu.io>
