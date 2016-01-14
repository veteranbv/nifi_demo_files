# nifi_demo_files
Couple of things to be aware of:
Template
The Solr location is set to sandbox.hortonworks.com:2181 (zookeeper url)
Dashboard
There’s a Solr JSON object configured as such
"solr": {
    "server": "http://sandbox.hortonworks.com:8983/solr/",
    "core_name": "tweets",
    "core_list": [
      "tweets_shard1_replica1"
    ],
    "global_params": "&df=id"
  }

Each will need to be customized for your environment.
