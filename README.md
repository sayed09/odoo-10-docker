# Docker To Setup Odoo 10 With pgAdmin Access


### Install docker:
```
$ sudo apt install docker.io
$ sudo systemctl start docker
$ sudo systemctl enable docker
```

### Install docker compose:
```
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.23.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
$ sudo systemctl enable docker
```

### Start the container from the root of this project:
```
$ docker-compose up  -d
```

Then locate `localhost:10000` to access Odoo 10.0.

And locate `localhost:5050` to access pgAdmin using the following credentials.
```
user: admin@admin.com
password: admin
```
