#  🔥RUNNING DEEPSEEK AI ON LOCAL SERVER USING DOCKER CONTAINER

- download the repo:
    ```bash
    git clone https://github.com/limmmw/docker-deepseek.git
    cd docker-deepseek
    ```
- run: 
    ```bash
    docker-compose up -d
    ```
- access ```http://localhost:3000```

- stop:
    ```bash
    docker-compose down
    ```
## REVERSE PROXY [OPTIONAL]
if you want to use reverse proxy with nginx in your system, use ai.conf file

```bash
sudo cp ai.conf /etc/nginx/sites-available/
sudo ln -s /etc/nginx/sites-available/ai.conf /etc/nginx/sites-enabled/ai.conf
sudo nginx -t
sudo systemctl reload nginx
```

then you can access the web with ```http://localhost``` or if you want to set with local domain on ```/etc/hosts```