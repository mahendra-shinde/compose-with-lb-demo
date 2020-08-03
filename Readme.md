# Docker-Compose with NGINX Load Balancer demo

1. Download this demo with parent folder 'compose-with-lb-demo'

2. Using CMD or POWERSHELL (Use bash on Linux/Mac), launch solution with 3 copies for 'app' service.

```
$ docker-compose up --scale app=3 -d 
$ docker-compose ps
```

3. Test by making multiple requests to URL http://localhost:8080

```
## On Windows Using powershell (Please repeat command at least THREE times)
$ iwr -UseBasicParsing http://localhost:8080

## On Linux or Mac using Bash (Please repeat command at least THREE times)
$ curl -v http://localhost:8080
```

4. You could test URL 'http://localhotst:8080' using multiple browsers (Web browser might CACHE the page, and may show same output even if serve by different instance).

