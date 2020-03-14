# elasticsearch-test-cluster

This is a dev cluster to study the *Elasticsearch Engineer I Course*. The original datasets from the course are automatically pushed to the Elasticsearch cluster.

- Uncompress the datasets
`tar -xvf sources/datasets.tar.gz`
- Deploy the cluster
`docker-compose up`
- Open *localhost:5601* for Kibana

Run your Elasticsearch queries from Kibana Dev Tool or using *curl localhost:9200*.

Logstash will push 1254941 docs to Elasticsearch, it takes some time. Check the progress running `curl -s localhost:9200/_count | jq -r '.count'`
