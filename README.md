# [Gogs](https://gogs.io/) running with Docker Compose

## Usage

### How to start
---
1. Clone this repo.
1. Set value for the `SECRET_KEY` in the `data\config\app.ini` (e.g. using [www.random.org](https://www.random.org/strings/?num=1&len=15&digits=on&upperalpha=on&loweralpha=on&unique=off&format=html&rnd=new)).
2. Run `docker-compose up -d` to start gogs.
3. To check that your gogs application is running enter url [http://localhost:3000](http://localhost:3000) (`ROOT_URL`).
4. Register a new user account.

### How to close 
---

1. Run `docker-compose stop` to stop gogs container.
2. Run `docker-compose rm -f` to remove gogs container.
3. Remove all files from `data/data`, `data/log`, `repo` and `ssh` folders.

## Settings

See the [Gogs configuration cheat sheet][1] for more information.

[1]: https://github.com/gogs/docs/blob/master/en-US/advanced/configuration_cheat_sheet.md "Gogs cheat sheet"
