# ansible-nextcloud-containerized

An all-in-one nextcloud deployment using nginx, mariadb, smtp in docker containers.

Other variables can be set in defaults/all.yml file:

```
nextcloud:
  db_volume: "db"
  mysql_db_name: "db"
  mysql_db_pw: "super_secret2"
  mysql_db_user: "nextcloud"
  mysql_root_pw: "super_secret"
  mysql_container_image: "mariadb"
  mysql_container_tag: "latest"
  nextcloud_container_image: "nextcloud"
  nextcloud_container_tag: "latest"
  nginx_container_image: "mariadb"
  nginx_container_tag: "latest"
  nginx_domain_name: "localhost"
  nginx_pem_volume: "/var/ansible/self-signed:/etc/nginx/ssl.pem:ro"
  restart_policy: "always"
  smtp_container_image: "mariadb"
  smtp_container_tag: "latest"
  state: "started"
  volume: "nextcloud"
```
