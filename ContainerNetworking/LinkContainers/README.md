# Link Two Containers.

# Create a Link

# 1. Create source container first
# 2. Create the recipient container and use the --link option

# Create the source containder using the postgres database
sudo docker run -d --name dbms postgres

# Create the recipient container and link it 
sudo docker run -it --name website --link dbms:db ubuntu:14.04 bash

















