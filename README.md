## Description
POC for how to apply a Self-Signed HTTPS Certificate to Nginx.

## quickstart

```bash
git clone https://github.com/selfcertificationhub/nginx-certificate.git
cd nginx-certificate
docker compose -f docker-compose.yml up -d
```

- `-d` flag runs the container in detached mode (in the background).

Afterward, when you access https://localhost/ in your browser, you'll be greeted with the message "Hello nginx!"

You have the option to utilize the default certificate or create a new one that shares the same IP address, namely "172.23.0.2".

Furthermore, you're able to modify the default IP, for instance, change it to "172.23.0.3" or select any other within the subnet: 172.23.0.0/16. However, remember to substitute the old IP in both the nginx.conf and docker-compose.yml files.

Good luck!

## Quick reference
- [issue #1 : how to use it with nginx](https://github.com/selfcertificationhub/selfcertificationhub/issues/1)