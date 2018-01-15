# rakam-io-demo

A simple demo of how to use rakam.io OSS projetc for gathering end users facts & metrics

# usage

1. `docker run -d --name rakam-db -e POSTGRES_PASSWORD=dummy -e POSTGRES_USER=rakam postgres:10.1 && docker run --link rakam-db --name rakam -p 9999:9999 -e RAKAM_CONFIG_LOCK__KEY=mylockKey -e RAKAM_CONFIG_STORE_ADAPTER_POSTGRESQL_URL=postgres://rakam:dummy@rakam-db:5432/rakam buremba/rakam`
2. go to https://app.rakam.io and register your cluster
3. generate a new project
4. find you api keys
5. replace it in the html
6. hit a bunch of refresh on the `yabon.html` web page
