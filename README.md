# node-firefox-debug

Docker container for creating a selenium node with Firefox, only for development.
[![](https://images.microbadger.com/badges/image/wywincl/node-firefox-debug.svg)](http://microbadger.com/images/wywincl/node-firefox-debug "Get your own image badge on microbadger.com")

# usage

### images

```
docker pull selenium/hub

docker pull wywincl/node-firefox-debug
```
### run
```
docker run -d -p 4444:4444 --name selenium-hub selenium/hub
docker run -d -P -p 5901:5900 --name selenium-node-firefox --link selenium-hub:hub wywincl/node-firefox-debug
```
