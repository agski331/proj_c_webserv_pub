To deploy this setup to a new server, do the following:
Clone the playbook, playbook.yml onto the new server.
install ansible onto this server
run this command as root: ansible-playbook playbook.yml

A modsecurity proxy should be running on port 8080 HTTP
A nginx proxy should be running on HTTPS port 443
A DVWA box should be running on port 80 on the internal docker network, inaccessible to the host.

To tear down the boxes, navigate to the directory where the docker-compose file is and type
docker-compose down
