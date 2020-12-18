# Caching Redis Node

The process of caching with Redis is quite simple. When we receive a user request to a route that has caching enabled, we first check if the requested data is already stored in the cache. If yes, we can quickly retrieve data from Redis and send the response.

## Setup redis locally

- wget http://download.redis.io/redis-stable.tar.gz
- tar xvzf redis-stable.tar.gz
- cd redis-stable
- make
- sudo make install
- start the redis server using `redis-server`
- test using `redis-cli ping`

### API

- using the Github Jobs API to get data related to programming jobs available in the different locations in the world.
- Run the local server and add the url in this format `http://localhost:3000/jobs?search=nodejs`