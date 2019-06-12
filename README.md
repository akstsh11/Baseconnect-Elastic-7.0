# Baseconnect-Elastic-7.0

## 起動方法
```
##　git clone する
$ git clone git@github.com:akstsh11/Baseconnect-Elastic-7.0.git
$ cd Baseconnect-Elastic-7.0

## Dockerイメージをビルドする
$ docker-compose build

## コンテナ起動
$ docker-compose up
```

## Elasticsearchに接続
``` http://localhost:9200 ```にアクセスし、以下のようなjsonデータが表示されたらok

```
{
  "name" : "1dbbacd31971",
  "cluster_name" : "docker-cluster",
  "cluster_uuid" : "CfVW5wzLTn6_99ygh0w7Dg",
  "version" : {
    "number" : "7.0.1",
    "build_flavor" : "default",
    "build_type" : "docker",
    "build_hash" : "e4efcb5",
    "build_date" : "2019-04-29T12:56:03.145736Z",
    "build_snapshot" : false,
    "lucene_version" : "8.0.0",
    "minimum_wire_compatibility_version" : "6.7.0",
    "minimum_index_compatibility_version" : "6.0.0-beta1"
  },
  "tagline" : "You Know, for Search"
}
```

## Kibanaに接続
``` http://localhost:5601 ```にアクセスする