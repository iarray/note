```
docker run -d --hostname my-rabbit --name my-rabbit -p 8787:15672 -p 1883:1883 -p 5672:5672 -e RABBITMQ_DEFAULT_USER=test -e RABBITMQ_DEFAULT_PASS=123456 rabbitmq:3-management

docker exec <容器ID> rabbitmq-plugins list

docker exec <容器ID> rabbitmq-plugins enable rabbitmq_web_mqtt

```

5672 是AMQP的连接端口

15672是rabbit的web管理端口

1883是mqtt的tcp连接端口

15675是mqtt的web管理端口