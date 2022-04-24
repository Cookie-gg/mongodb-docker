# a image of mongodb in docker

### setup
- make a image
```
docker-compose up -d
```

- setup of replica
```
docker-compose exec mongodb mongo --eval "rs.initiate({_id: 'rs0', members: [{_id: 0, host: 'localhost:27017'}]});"
```