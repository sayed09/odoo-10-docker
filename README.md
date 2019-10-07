# Setup Docker for Odoo 10 Community or Enterprise Version


Install docker:
```
$ sudo apt install docker.io
$ sudo systemctl start docker
$ sudo systemctl enable docker
```

Install docker compose:
```
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.23.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
$ sudo systemctl enable docker
```

Start the container:
```
$ docker-compose up
```

Then locate `localhost:10000` to access Odoo 10.0.

And locate `localhost:5555` to access pgAdmin using the following credentials.
```
user: admin@pgadmin.com
password: 123456
```

If you want to run in detached mode, execute this command:
```
$ docker-compose up -d
```
