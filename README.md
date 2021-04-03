# Initial Instructions
Install docker and docker-compose in your machine

# Run command to rename .env
cp env.dist .env

# Run command to up containers
docker-compose up -d
docker container restart nginx

# Add host /etc/hosts with sudo
127.0.0.1 index.local

# Test network beetween nginx and msyql containers
docker exec -ti nginx bash -c "ping mysql"

# Test app in browser
http://index.local