# Docker Play Launchers <a href="https://labs.play-with-docker.com/" target="_blank"><img src="https://cdn.rawgit.com/play-with-docker/stacks/cff22438/assets/images/button.png" alt="Try in PWD"></a>

Play With Docker: https://labs.play-with-docker.com/ ( https://labs.play-with-docker.com?stack= )
<br>Docker Playground Guide: https://www.guschlbauer.dev/play-with-docker-pwd-an-amazing-one-click-docker-playground-project/
<br>YAML in 5 minutes: https://www.codeproject.com/Articles/1214409/Learn-YAML-in-five-minutes

Portainer-ce: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/Portainer.yml" target="new">PWD => Portainer.yml</a> (admin/password)
<br>Filebrowser: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/Filebrowser.yml" target="_blank">PWD => Filebrowser.yml</a>
<br>Portainer + Filebrowser: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/stack.yml" target="_blank">PWD => stack.yml</a>
<br>ToDo stacks:
<br>Portainer + FileBrowser + PostgreSQL + pgWeb/Adminer;

_
<br>MySQL+phpMyAdmin: https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/play-with-docker/stacks/master/mysql/latest/stack.yml
<br>PostgreSQL+pgWeb: https://labs.play-with-docker.com/?stack=https://raw.githubusercontent.com/play-with-docker/stacks/master/postgres/latest/stack.yml (pgWeb container lives for 1s, then "docker ps" is empty!)

_


Docker Play workspace:
<br>docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock --name portainer portainer/portainer
<br>docker run -d -p 8080:80 -v /:/srv/ --name filebrowser filebrowser/filebrowser (admin/admin)
