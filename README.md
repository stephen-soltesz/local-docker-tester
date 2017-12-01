# local-docker-tester

```

docker build -t local-cloud-sdk .
docker run -it --name bq-exporter -p 9393:9393 --rm \
    --volumes-from gcloud-config \
    -w /go \
    -v $HOME/linux-src:/go/src \
    -v $PWD:/go/src/github.com/m-lab/prometheus-bigquery-exporter \
    local-cloud-sdk /bin/bash

```
