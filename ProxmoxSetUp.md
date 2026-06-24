# how to setup docker using proxmox LXC

in proxmox shell enter this:
> pct set <CTID> -features nesting=1,keyctl=1
> pct set <CTID> -unprivileged 0

in the container shell enter
if you havent already, install curl:
> apt install curl

> curl -fsSL https://get.docker.com | sh