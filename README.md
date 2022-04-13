setup:  
```
# install rabbitmq on ubuntu
chmod +x insatll.sh
./install.sh

# add user
sudo rabbitmqctl add_user bb
sudo rabbitmqctl set_user_tags bb administrator
sudo rabbitmqctl set_permissions -p / bb ".*" ".*" ".*"


# activate plugin
rabbitmq-plugins enable rabbitmq_web_stomp

# open azure ports in network security group

```

ressources
https://www.rabbitmq.com/web-stomp.html  

