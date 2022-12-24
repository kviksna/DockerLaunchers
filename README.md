# Docker Play Launchers <a href="https://labs.play-with-docker.com/" target="_blank"><img src="https://cdn.rawgit.com/play-with-docker/stacks/cff22438/assets/images/button.png" alt="Try in PWD"></a>

Play With Docker(PWD): https://labs.play-with-docker.com/ ( https://labs.play-with-docker.com?stack= )
<br>Docker Playground Guide: https://www.guschlbauer.dev/play-with-docker-pwd-an-amazing-one-click-docker-playground-project/
<br>YAML in 5 minutes: https://www.codeproject.com/Articles/1214409/Learn-YAML-in-five-minutes
<br>Docker images: https://hub.docker.com/

Portainer-ce: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/Portainer.yml" target="new">PWD => Portainer.yml</a> (admin/password)
<br>Filebrowser: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/Filebrowser.yml" target="_blank">PWD => Filebrowser.yml</a>
<br>Portainer + Filebrowser: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/portainer-filebrowser.yml.yml" target="_blank">PWD => portainer-filebrowser.yml</a>
<br>Postgres + pgWeb: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/pg-pgweb.yml" target="_blank">PWD => pg-pgweb.yml</a>
<br>Postgres + pgAdmin4: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/pg-pgadmin.yml" target="_blank">PWD => pg-pgadmin.yml</a>
<br>MySQL+phpMyAdmin: https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/play-with-docker/stacks/master/mysql/latest/stack.yml
<br>Stack: Portainer + FileBrowser + PostgreSQL + pgAdmin4 (phpPgAdmin/Adminer/pgWeb)

_

Docker Play workspace:
<br>docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock --name portainer portainer/portainer
<br>docker run -d -p 8080:80 -v /:/srv/ --name filebrowser filebrowser/filebrowser (admin/admin)
<br>docker run -d -p 80:80 -e 'PGADMIN_DEFAULT_EMAIL=user@domain.com' -e 'PGADMIN_DEFAULT_PASSWORD=SuperSecret' dpage/pgadmin4
