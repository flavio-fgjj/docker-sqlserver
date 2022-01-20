<h1 align="center">SQL Server Docker</h1>

# docker-sqlserver
<p align="left">subindo um container sql server no docker</p>

# Obtendo a imagem
$ docker pull mcr.microsoft.com/mssql/server:latest
  
# Rodando o SQL Server (coloque uma senha segura)
$ docker run --name sqlserver -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=123456" -p 1433:1433 -d mcr.microsoft.com/mssql/server

# Connection String 
<!--ts-->
   * Não se esqueça de colocar a mesma senha que foi colocada no "docker run"
<!--te-->
<code>Server=localhost,1433;Database=seudatabase;User ID=sa;Password=123456</code>

Fonte:
[Blog do Balta](https://balta.io/blog/sql-server-docker).
