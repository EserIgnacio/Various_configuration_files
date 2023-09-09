# Various_configuration_files

### Sample .bashrc Configuration

Example `.bashrc` configuration file with custom PATH and aliases:

```bash
# Setting PATH
export PATH=$PATH:/usr/local/bin:/opt/bin

# Aliases
alias ll='ls -l'
alias ..='cd ..'

---

### Sample Nginx Server Block Configuration

Example Nginx server block configuration for `example.com`:

```nginx
server {
    listen 80;
    server_name example.com www.example.com;

    location / {
        proxy_pass http://backend_server;
    }
}

---

### Sample Docker Compose Configuration

Example Docker Compose configuration for running Nginx and a custom app:

```yaml
version: '3'
services:
  web:
    image: nginx:latest
    ports:
      - "80:80"
  app:
    image: my-app:latest

---

### Sample Docker Compose Configuration

Example Docker Compose configuration for running Nginx and a custom app:

```yaml
version: '3'
services:
  web:
    image: nginx:latest
    ports:
      - "80:80"
  app:
    image: my-app:latest


---

### Sample MySQL Configuration

Example MySQL configuration in `my.cnf`:

```ini
[mysqld]
datadir=/var/lib/mysql
socket=/var/lib/mysql/mysql.sock
user=mysql
# ...

---

### Sample SSH Configuration

Example SSH server configuration in `sshd_config`:

```ssh
Port 22
PermitRootLogin no
PasswordAuthentication yes
