# Hands-on Go AMQP

### Simple consumer and producer

```bash
$> go run send_receive/send/send.go

2022/02/20 14:12:41 [X] Sent Hello World!
```
```bash
$> go run send_receive/receive/receive.go

2022/02/20 14:13:01 [*] Waiting for messages. To exit press CTRL+C
2022/02/20 14:13:01 Received a message: Hello World!
```

### Worker queue

```bash
$> go run worker_queues/new_task/new_task.go

2022/02/20 14:25:07 [X] Sent hello
```
```bash
$> go run worker_queues/worker/worker.go

2022/02/20 14:25:38 [*] Waiting for messages. To exit press Ctrl+C
2022/02/20 14:25:38 Received a message: hello
2022/02/20 14:25:38 Done
```

### Publisher and subscriber

```bash
$> go run publish_subscribe/emit_log/emit_log.go

2022/02/20 16:54:11 [X] Sent hello
```
```bash
$> go run publish_subscribe/receive_logs/receive_logs.go

2022/02/20 16:53:59 [*] Waiting for logs. To exit press CTRL+C
2022/02/20 16:54:11 [X] hello
```
