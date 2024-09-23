# IMPORTANT
```
git clone https://github.com/mailcow/mailcow-dockerized
```
```
cd mailcow-dockerized
```
```
./generate_config.sh
```
Europe/Berlin

```
nano mailcow.conf
```
# add following line (root domain)
DOMAIN= 

HTTP_PORT=7083
HTTP_BIND=127.0.0.1

HTTPS_PORT=7443
HTTPS_BIND=127.0.0.1

ADDITIONAL_SAN=imap.*,smtp.*,mail.*
ADDITIONAL_SERVER_NAMES=mail.mydomain.com

SKIP_LETS_ENCRYPT=y

#FLATCURVE_EXPERIMENTAL=y
```
sudo lsof -i -P -n | grep LISTEN
```
```
nano docker-compose.override.yml
```

### DOMAIN anpassen