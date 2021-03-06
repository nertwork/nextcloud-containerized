# ansible-nextcloud-containerized

An all-in-one nextcloud deployment using nginx, mariadb, smtp in docker containers.

Other variables can be set in [defaults/main.yml](defaults/main.yml) file:

```
nextcloud:
  db_volume: "db"
  mysql_container_image: "mariadb"
  mysql_container_tag: "latest"
  mysql_db: "nextcloud"
  mysql_db_name: "db"
  mysql_db_pw: "super_secret2"
  mysql_db_user: "nextcloud"
  mysql_root_pw: "super_secret"
  nextcloud_container_image: "nextcloud"
  nextcloud_container_tag: "latest"
  nginx_container_image: "nginx"
  nginx_container_tag: "latest"
  nginx_fqdn: "localhost.localhost"
  nginx_pem_volume: "/var/ansible/self-signed:/etc/nginx/ssl.pem:ro"
  restart_policy: "always"
  smtp_container_image: "namshi/smtp"
  smtp_container_tag: "latest"
  state: "started"
  volume: "nextcloud"
```
