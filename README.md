## About

This project demonstrates a basic setup and control flow for managing an NGINX web server locally, including starting, stopping, reloading the service, viewing access logs, and enabling HTTPS with a self-signed SSL certificate.

## Key features

- Start, stop, and reload NGINX using command-line tools.
- View real-time access logs for monitoring incoming requests.
- Create a self-signed SSL certificate for local HTTPS support.
- Organize and store certificates in a dedicated directory (~/nginx-certs).

### Commands used

##### start nginx

`nginx`

##### get options

`nginx -h`

##### restart nginx

`nginx -s reload`

##### stop nginx

`nginx -s stop`

##### print logs

`tail -f /usr/local/var/log/nginx/access.log`

##### restart nginx

`nginx -s reload`

##### create folder for nginx certificates

`mkdir ~/nginx-certs`
`cd ~/nginx-certs`

##### create self-signed certificate

`openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout nginx-selfsigned.key -out nginx-selfsigned.crt`
