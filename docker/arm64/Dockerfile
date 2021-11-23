FROM arm64v8/rabbitmq:3.9-management

LABEL version="arm64v1.0.0"
LABEL Christian Sargusingh "https://github.com/cSDes1gn"

# package custom config
ADD rabbitmq/rabbitmq.conf /etc/rabbitmq/
ADD rabbitmq/definitions.json /etc/rabbitmq/
ADD rabbitmq/enabled_plugins /etc/rabbitmq/

CMD ["rabbitmq-server"]