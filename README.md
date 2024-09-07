# SQL Server
### Run and go Docker setup for SQL Server.

<br />

To start SQL Server on background via Docker just type:
```
docker compose up -d
```

Main parameters can be modified via `.env` file.


Default configuration:
```
IMAGE: mcr.microsoft.com/mssql/server:2022-latest
CONTAINER NAME: sqlserver
USER: sa
PASSWORD: A123456*
PORT: 1433 (default for SQL Server)
```

Data are persisted locally:
```
./volumes/mssql/data
```

Connection via SQL Server Management Studio:
```
Server type: Database Engine
Server name: localhost
Authentication: SQL Server Authentication
Login: sa
Password: A123456*
```

Docker network:
```
sqlserver
```