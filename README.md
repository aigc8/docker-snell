:whale: Dockerfiles for [snell](https://manual.nssurge.com/others/snell.html) with [glibc](https://github.com/sgerrand/alpine-pkg-glibc)


docker run -d \
  --name snell-server \
  -p 6160:6160 \
  -e INTERFACE=0.0.0.0 \
  -e PORT=6160 \
  -e PSK=your_psk_here \
  -e IPV6=false \
  --restart unless-stopped \
  blackmini/snell-server
