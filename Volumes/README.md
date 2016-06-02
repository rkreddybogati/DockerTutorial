# This is tutorial on Volumes.

# Volumes are mounted when creating and executing container
# Can be mapped to hostdirectly 
# Volume paths specified must me absolute


# Execute new container and mount the folder /nginx13volume into its file system
sudo docker run -d -P -v /nginx13volume nginx

# Execute new container and map /data/src from host into /test/src folder in container 
sudo docker run -i -t -v /data/src:/test/src nginx

# Volumes in Dockerfile
# String Example
VOLUME /myvol

# String Example with multiple volumes
VOLUME /myvol1 /myvol2

# JSON Example 
VOLUME [ "myvol1", "myvol2" ]


# Create and Test a Volume

# 1. Execute a new container and initialise volume at /www/website. Run a bash terminal as your container process
sudo docker run -i -t -v /www/website nginx bash

# 2. Inside the container verify that you can go to /www/website

# 3. Create a file inside /www/website folder
# 4. Exit the container
# 5. Stop and Commit the updated container as new images calles some test:1.0 
sudo docker commit <ContaindeID> test:1.0

# 6. Execute the new container with your test image and go to it's bash shell
sudo docker run -i -t test:1.0 bash

# 7. Verify that the /www/website folder exists and that there are no files inside. 




