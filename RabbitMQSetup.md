# Accessing RabbitMQ Management Plugin on Port 15672

Follow the steps below to enable and access the RabbitMQ Management Plugin on port 15672 after installing RabbitMQ and Erlang on your Windows machine.

## 1. Enable the RabbitMQ Management Plugin
   By default, the RabbitMQ Management Plugin is disabled. To enable it:

1. Open a command prompt as Administrator.
2. Run the following command:
```bash
rabbitmq-plugins enable rabbitmq_management
```

This will enable the RabbitMQ Management Plugin, providing a web-based UI, HTTP API, and more.

## 2. Restart RabbitMQ Service (If Required)
You may need to restart the RabbitMQ service for the changes to take effect.

* Open Services (search for it in the Start Menu).
* Find the RabbitMQ service.
* Right-click on it and choose Restart.

Alternatively, you can restart RabbitMQ from the command line:
```bash
rabbitmqctl stop
rabbitmq-server start
```

## 3. Access RabbitMQ Management Console
Once the plugin is enabled and RabbitMQ is running, open your web browser and go to:
```bash
http://localhost:15672
```

## 4. Login to RabbitMQ Management
* Username `guest`
* Password: `guest`