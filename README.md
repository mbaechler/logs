# Logs

This project aims at analysing logs from ideasbox instances to discover how
users interact with the software.

It's based on the famous ELK stack and Docker.

## Requirements

You need Docker, docker-compose and htpasswd from apache2-utils.

## How to use it

You need two things : some logs and an htpasswd file to protect your instance
from evil hackers.

You can generate your htpasswd file by doing :

	htpasswd -c htpasswd <username>

Then you just have to type :

	docker-compose build
	docker-compose up
