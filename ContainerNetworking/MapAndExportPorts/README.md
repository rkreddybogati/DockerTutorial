# Container Networking Basics. 

# Mapping Ports
# Map port 80 on the container to 8080 port on host machine
sudo docker run -d -p 8080:80 nginx

# Automapping ports
# Use the -P option in docker run.
# It automatically maps ports in container to the port number in host
# Host port numbers used from 49153 to 65535
# Only works for the ports definde in the EXPOSE instruction

# Auto map ports exposed by NGINX container to a port value on the host 
sudo docker run -d -P nginx:1.7

# EXPOSE instruction
# Configure which ports a container will listern on at run time 
# Ports still need to mapped when container is executed
# See Dockerfile unser Expose folder here. 



