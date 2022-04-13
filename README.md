http://ml-server.westeurope.cloudapp.azure.com:12333/  
open multiple tabs for more fun

rabbitmq server is deployed on azure VM and it communicates with websockets with clien's interface.  
web server is deployed with lighttpd with azure VM on port 12333.  



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

