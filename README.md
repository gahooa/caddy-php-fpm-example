# caddy-php-fpm-example
A transient example of Caddy and PHP-FPM

# The problem

Browser -> Caddy -> PHP FPM is working

However, the only response is 404 not found.

# To run

Make sure nothing is using port 80 or 443 on your local computer.

`docker compose build`  
`docker compose up`

Visit https://local.ehw2.net

(This resolves to 127.0.0.1)

# Objectives 

1. php-fpm shoud serve from /App/Web/
2. Get phpinfo() working from /App/Web/index.php
3. Consolodate php-fpm.conf to a single file and write to the container 


