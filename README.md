# Projeto de Sistemas Distribuídos 2015-2016 #

Grupo de SD 44 - Campus Alameda

José Semedo   78294 jose.francisco.semedo@gmail.com

Lídia Freitas 78559 lidiamcfreitas@gmail.com

João Marçal   78471 joao.marcal12@gmail.com


Repositório:
[tecnico-distsys/A_44-project](https://github.com/tecnico-distsys/A_44-project)

-------------------------------------------------------------------------------

## Instruções de instalação 


### Ambiente

[0] Iniciar sistema operativo

Linux


[1] Iniciar servidores de apoio

JUDDI:
```
O servidor de nomes a utilizar é o jUDDI (Java UDDI).
Para lançar o servidor, basta executar o seguinte comando na pasta juddi-.../bin:
 $./startup.sh (Linux e Mac)
 $./startup.bat (Windows)
```


[2] Criar pasta temporária

```
cd ~
mkdir Project
```


[3] Obter código fonte do projeto (versão entregue)

```
git clone  https://github.com/tecnico-distsys/A_44-project.git
```
*(colocar aqui comandos git para obter a versão entregue a partir da tag e depois apagar esta linha)*


[4] Instalar módulos de bibliotecas auxiliares

```
cd uddi-naming
mvn clean install
```

-------------------------------------------------------------------------------

### Serviço TRANSPORTER

[1] Construir e executar **servidor**

```
cd transporter-ws
mvn clean install
mvn exec:java
```

[2] Construir **cliente** e executar testes

```
cd transporter-ws-cli
mvn clean install
```



-------------------------------------------------------------------------------

### Serviço BROKER

[1] Construir e executar **servidor**

```
cd broker-ws
mvn clean install
mvn exec:java
```


[2] Construir **cliente** e executar testes

```
cd broker-ws-cli
mvn clean install
```


-------------------------------------------------------------------------------
**FIM**
