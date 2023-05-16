## nginx-html
Static website bootstrapped with Docker nginx.

## Commands
```bash
# pull latest nginx image
docker pull nginx:latest

# bootstrap a nginx server with docker( http://localhost:8000/ )
docker run -it -p 8000:80 nginx

# display & remove exited container
docker ps -a
docker rm 0116feb446c9

# run docker nginx in background
docker run -d -p 8000:80 -v /Users/chen/nginx-html:/usr/share/nginx/html --name my-nginx nginx

# static html page is available now
Index: http://localhost:8000/
About: http://localhost:8000/about.html

# stop your docker container
By name: docker stop my-nginx
By containerid: docker stop e71175fcf96d
```

## License
MIT