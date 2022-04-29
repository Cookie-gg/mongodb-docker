# mongodb - docker container for development

### setup
- make a image
```
docker-compose up -d
```

- setup for replica
```
docker-compose exec mongodb mongo --eval "rs.initiate({_id: 'rs0', members: [{_id: 0, host: 'localhost:27017'}]});"
```