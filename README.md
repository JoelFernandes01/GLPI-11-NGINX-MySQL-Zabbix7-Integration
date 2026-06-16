# GLPI-11-NGINX-MySQL-Zabbix7-Integration
## Instalar o GLPI no Ubuntu - NGINX + MySQL

### Atualizar o sistema operacional Ubuntu 26.04
```bash
sudo apt update && sudo apt install -y
```
### Instalar o PHP e as extensões necessárias e o banco MySQL
```bash
sudo apt install mysql-server php-{cli,ldap,xmlrpc,soap,curl,snmp,zip,apcu,gd,mbstring,mysql,xml,bz2,intl,bcmath} -y
```
### Instalar o NGINX ( https://nginx.org/en/linux_packages.html#Ubuntu )
```bash
sudo apt install curl gnupg2 ca-certificates lsb-release ubuntu-keyring -y
```
### Verficar as chaves 
```bash
curl https://nginx.org/keys/nginx_signing.key | gpg --dearmor \
    | sudo tee /usr/share/keyrings/nginx-archive-keyring.gpg >/dev/null
```bash
gpg --dry-run --quiet --no-keyring --import --import-options import-show /usr/share/keyrings/nginx-archive-keyring.gpg
```
### Atualizar os pacotes e instalar o NGINX
```bash
sudo apt update -y
sudo apt install nginx -y
```


### Criar o banco de dados e o usuário glpi
```bash
mysql -u root -e "create database gpldb character set utf8;"
mysql -u root -e "create user 'gpl'@'localhost' identified by '123@Mudar';"
mysql -u root -e "grant all privileges on gpldb.* to 'gpl'@'localhost' with grant option;"
mysql -u root -e "flush privileges;"
```

### Baixando e instalando o GLPI ( https://github.com/glpi-project/glpi/releases )
```bash
wget https://github.com/glpi-project/glpi/releases/download/11.0.7/glpi-11.0.7.tgz
```


