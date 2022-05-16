# custom-es-cluster-in-docker-compose


一个自定义的基于 docker compose 的 es 集群

```bash
# 启动和销毁 compose stack
docker-compose up -d
docker-compose down -v
```

我们有两种方法来管理这些服务：

1. 在 docker-compose.yml 里修改环境变量，改变 es 节点的行为。
2. 使用一些单独的文件夹，如 es1、es2、e3、等文件夹专门管理内外数据卷或者配置文件-配置文件里的配置应该可以覆盖环境变量的配置