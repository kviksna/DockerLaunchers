# Play With Docker(PWD) <a href="https://labs.play-with-docker.com/" target="_blank"><img src="https://cdn.rawgit.com/play-with-docker/stacks/cff22438/assets/images/button.png" alt="Try in PWD"></a>

<br>https://labs.play-with-docker.com/ ( https://labs.play-with-docker.com?stack= )
<br><a href="https://www.guschlbauer.dev/play-with-docker-pwd-an-amazing-one-click-docker-playground-project/">Docker Playground Guide</a>, 
<a href="https://www.codeproject.com/Articles/1214409/Learn-YAML-in-five-minutes">YAML in 5 minutes</a>, https://hub.docker.com/

Portainer-ce: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/Portainer.yml" target="new">PWD => Portainer.yml</a>
<br>Filebrowser: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/Filebrowser.yml" target="_blank">PWD => Filebrowser.yml</a>
<br>Portainer + Filebrowser: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/portainer-filebrowser.yml.yml" target="_blank">PWD => portainer-filebrowser.yml</a>
<br>Postgres + pgWeb: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/pg-pgweb.yml" target="_blank">PWD => pg-pgweb.yml</a>
<br>Postgres + pgAdmin4: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/pg-pgadmin.yml" target="_blank">PWD => pg-pgadmin.yml</a>
<br>MySQL+phpMyAdmin: <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/mysql-phpmyadmin.yml" target="_blank">PWD => mysql-phpmyadmin.yml</a>
<br>Stack: Portainer + FileBrowser + PostgreSQL + pgAdmin4 (phpPgAdmin/Adminer/pgWeb): <a href="https://labs.play-with-docker.com?stack=https://raw.githubusercontent.com/kviksna/DockerLaunchers/main/stack.yml" target="_blank">PWD => stack.yml</a> (PWD ar šo netiek galā !  Sintakse ir korekta!)


Docker Play workspace:
<br>docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock --name portainer portainer/portainer
<br>docker run -d -p 8080:80 -v /:/srv/ --name filebrowser filebrowser/filebrowser (admin/admin)

https://www.pgadmin.org/docs/pgadmin4/latest/container_deployment.html
<br>docker run -d -p 80:80 -e 'PGADMIN_DEFAULT_EMAIL=user@domain.com' -e 'PGADMIN_DEFAULT_PASSWORD=SuperSecret' dpage/pgadmin4

Stack working deployent:
<br>1. Open and login to https://labs.play-with-docker.com/
<br>2. [New Instance]
<br>3. Run docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock --name portainer portainer/portainer
<br>4. Open :9090 port
<br>5. Set Portainers new user pwd 12 symbols (for exaple: adminadminadmin)
<br>6. In Portainer UI: Home > local > Stacks > [+ Add stack] > Name: lowcase
<br>7. Web editor: docker-compose.yml contents
<br>8. Actions: [Deploy the stack]
<br>9. Containers > copy postgers IP
<br>10. Open :82 port to open pgAdmin4 UI (slow start -self refresh when ready, so just wait) (user@domain.com/SuperSecret)
<br>11. [Add new server] > General: Name:
<br>11. Host: postgres container IP (9.) postgres/postgres [Save]
<br>12. File > Pereferences > Miscellanious > Theme: Dark [Save]
