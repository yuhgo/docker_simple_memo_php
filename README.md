# コンテナ起動コマンド
### ディレクトリ移動
```
cd docker_simple_memo_php
```
### 起動
```
docker-compose -f .docker_memo/docker-compose.yml up -d
```
### 起動確認
```
docker ps
```
#### 起動後
```
$ docker ps
PORTS                                NAMES
 80/tcp, 0.0.0.0:8080->8080/tcp       php_simple_memo_nginx
 9000/tcp                             php_simple_memo_php
 0.0.0.0:8081->80/tcp                 php_simple_memo_phpmyadmin
 33060/tcp, 0.0.0.0:13306->3306/tcp   php_simple_memo_mysql
```


# コンテナ停止コマンド
### 停止
```
docker-compose -f .docker_memo/docker-compose.yml down
```
### 停止確認
```
docker ps
```
