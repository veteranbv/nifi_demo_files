# Nifi Twitter Streaming Demo Files

##Couple of things to be aware of:
* Template
    * The "Solr Location" is set to [sandbox.hortonworks.com:2181]. Nifi, in this case, is refering to the fqdn:port for the Zookeeper node used by Solr.
* Dashboard
    * There’s a Solr JSON object with the following configuration
```
        "solr": {
            "server": "http://sandbox.hortonworks.com:8983/solr/",
            "core_name": "tweets",
            "core_list": [
              "tweets_shard1_replica1"
            ],
            "global_params": "&df=id"
          }
```

Each will need to be customized for your environment.

This work builds on, and is derived from, Ali Bajwa's repository [https://github.com/abajwa-hw/ambari-nifi-service]
