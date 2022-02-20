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
