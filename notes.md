docker build -t mugaf/frontend -f Dockerfile.dev .
use specific docker file with -f

docker run -p 3000:3000 mugaf/frontend

docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app mugaf/frontend
using volume to immitate hot reload

docker-compose up
running docker with docker compose file

docker build -t mugaf/frontend -f Dockerfile.dev . 
docker run -it mugaf/frontend npm run test
above commands to run test