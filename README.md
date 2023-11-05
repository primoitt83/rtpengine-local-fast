# rtpengine-local-fast

Same as rtpengine-local but no compilation need it.

Rtpengine will be installed using precompiled deb files.

So it's a lot faster to build and run from Docker.

## How to test

- create a Ubuntu 18.04 (bionic) VM;
- disable ipv6;
- install docker;
- install docker-compose.

Local ip: 192.168.5.149

Create "net" network
````
docker network create --driver=bridge --subnet=172.25.0.0/16 net
````
Run this project:
````
cd /opt
git clone https://github.com/primoitt83/rtpengine-local-fast.git
cd rtpengine-local-fast
docker-compose up -d
````








