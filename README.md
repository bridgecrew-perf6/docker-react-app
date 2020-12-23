# Getting Started with Create React App in Docker

### Dev
```
  docker build -f Dockerfile.dev .
  docker run -it -p 3000:3000 -v /app/node_modules -v $(pwd):/app <image_id>
```

for tests use docker-compose:
```
  docker-compose up --build
  docker-compose down

```

### Prod with Nginx
```
  docker build .
  docker run -p 8080:80 <image_id>
```
