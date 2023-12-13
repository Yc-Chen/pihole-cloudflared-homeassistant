# Pi-hole, Cloudflared and Home Assistant

My setup is based on this blog: https://ben.balter.com/2021/09/01/how-i-re-over-engineered-my-home-network/

On top of it, I added

- Home Assistant
- macvlan (so that each docker container gets an IP in my home network, which works nicely if you combine it with DHCP from Pi-hole.)
- access to several USB ports

## To Upgrade

1. `docker-compose pull`
2. `docker-compose build`
3. `docker-compose up -d`
