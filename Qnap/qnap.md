Prerequisites: Containerstation is up and running
Open a ssh connection to your qnap and enter following command: 

`sudo docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=Passw0rd!' -p 1433:1433 -v /share/Container/sqlserver_data:/var/opt/mssql/data -v /share/Container/sqlserver_logs:/var/opt/mssql/log -v /share/Container/sqlserver_secrets:/var/opt/mssql/secrets -d mcr.microsoft.com/mssql/server:2019-latest`

You can verify your server has started and can connect using the following command:

`sudo docker container ls
`
and copy paste the id of your container: (e.g.)

`sudo docker exec -it a64f6540fef6 /opt/mssql-tools/bin/sqlcmd -S localhost -U sa -P Passw0rd!``

Further connectivity is discussed in a separate chapter: (see ...)