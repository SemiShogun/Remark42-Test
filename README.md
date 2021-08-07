# Remark42-Test
Testing out the remark42 comment engine by using Docker.

Please note that this repository utilizes Github OAuth, if you want to add other types of social media to this website, please refer to https://github.com/umputun/remark42#register-oauth2-providers.

## Requirements
- Docker
- A Github account

## Setup
1. Log in to Github and create a new "OAuth App" https://github.com/settings/developers
2. Fill down "http://localhost:8080" on Homepage URL and "http://localhost:8080/auth/github/callback" on Authorization callback URL. 
Feel free to give the Application name whichever name you want.
3. Locate the project and pull all of the Docker images 
```
docker-compose pull
```
4. Build the project 
```
docker-compose up --build
```

## How to use it
Simply type down localhost:8000 to access the website that is being run on the web container.
There you can try out remark42 by posting github comments.

If you want to access the remark42 instance directly, then head on over to localhost:8080/web.