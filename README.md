# verdaccio config

完整的实践记录，请访问 [blog](https://www.yuque.com/ubdme4/ccc/ogikut/) 获得更多参考。

## 使用

```shell
docker-compose up --build --force-recreate  -d
```

## 停止

```shell
docker-compose stop
```

## 没有 docker-compose

如果没有 docker-compose 的同学，也可以直接使用以下命令创建

```shell
docker run -d --name verdaccio \
-v $(pwd)/conf:/verdaccio/conf \
-v $(pwd)/storage:/verdaccio/storage \
-p 4873:4873 \
verdaccio/verdaccio
```
