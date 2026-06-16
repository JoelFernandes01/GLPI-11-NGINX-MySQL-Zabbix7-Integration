### Atualizar o sistema operacional Ubuntu 26.04
```bash
sudo apt update && sudo apt install -y
```
### Instalar o banco MySQL
```bash

```
### Baixar o repositório do Zabbix (  )
```bash

```

### Extrair o arquivo 
```bash

```

### Atualizar o repositório e instalar os pacotes
```bash
sudo apt update -y
```
```bash

```
### Criar o banco de dados e o usuário glpi
```bash
sudo mysql -u root -e "create database zabbixdb character set utf8;"
sudo mysql -u root -e "create user 'zabbix'@'localhost' identified by '123@Mudar';"
sudo mysql -u root -e "grant all privileges on zabbixdb.* to 'zabbix'@'localhost' with grant option;"
sudo mysql -u root -e "flush privileges;"
```


### Criar o arquivo de configuração do GLPI no NGINX
```bash
sudo vim /etc/nginx/sites-available/glpi.conf
```

### Copie e cole o conteúdo abaixo no arquivo criado acima
```bash

```

### Criando link simbólico para o arquivo de configuração do NGINX
```bash

```

### Verificar o NGINX
```bash

```

### Recarregar o NGINX
```bash

```

### Agora é acessar via browser o GLPI e iniciar o banco de dados .
```bash
http://zabbix.connect.local
```


## Figuras do Setup

| Imagem | Descrição |
|--------|-----------|
| [![Setup 01](figuras/SETUP-01.jpeg)](figuras/SETUP-01.jpeg) | Configuração inicial |
| [![Setup 02](figuras/SETUP-02.jpeg)](figuras/SETUP-02.jpeg) | Escolha da linguagem |
| [![Setup 03](figuras/SETUP-03.jpeg)](figuras/SETUP-03.jpeg) | Licença |
| [![Setup 04](figuras/SETUP-04.jpeg)](figuras/SETUP-04.jpeg) | Instalação ou Atualizção do GLPI |
| [![Setup 05](figuras/SETUP-05.jpeg)](figuras/SETUP-05.jpeg) | Check list do sistema |
| [![Setup 06](figuras/SETUP-06.jpeg)](figuras/SETUP-06.jpeg) | Conexão com o banco de dados |
| [![Setup 07](figuras/SETUP-07.jpeg)](figuras/SETUP-07.jpeg) | Teste de conexão com o banco de dados |
| [![Setup 08](figuras/SETUP-08.jpeg)](figuras/SETUP-08.jpeg) | Inicialização de todo o sistema |
| [![Setup 09](figuras/SETUP-09.jpeg)](figuras/SETUP-09.jpeg) | Dados coletados |
| [![Setup 10](figuras/SETUP-10.jpeg)](figuras/SETUP-10.jpeg) | Mensagem sobre GLPI-Network |
| [![Setup 11](figuras/SETUP-11.jpeg)](figuras/SETUP-11.jpeg) | A instalação está finalizada com sucesso |
| [![Setup 12](figuras/SETUP-12.jpeg)](figuras/SETUP-12.jpeg) | Tela de login |

### Fim do Processo de Instalação do Sistema GLPI ###
