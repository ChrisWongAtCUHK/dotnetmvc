# README

## Build
```
docker build -t dotnetmvc .
```

## Run
```
docker run -d -p 8080:80 dotnetmvc
```
http://localhost:8080/

## Deploy to Heroku
```
heroku container:login
heroku apps:create dotnetmvc
heroku container:push web --app dotnetmvc
heroku container:release web
```