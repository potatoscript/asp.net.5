# asp.net 5 Cheat Sheets:

| Title                                                                               | Remark/code              |
| ----------------------------------------------------------------------------------- | ------------------------ |
| [Entity Framework](https://github.com/potatoscript/asp.net.5/wiki/Entity-Framework) | Object-relational mapper |
| [OData](https://github.com/potatoscript/asp.net.5/wiki/odata)                       | Open data protocol       |

GETTING STARTED

- Make sure to install global EF tools: `dotnet tool install --global dotnet-ef`
- Run local SQL Server using Docker:
  - `docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=yourStrong(!)Password' -e 'MSSQL_PID=Express' -p 1433:1433 -d mcr.microsoft.com/mssql/server`
- Install and use free `SQL Server Developer Edition` or `SQL Server Express LocalDB`
- Use In-Memory DB for simple test scenarios

- Setup the `Azure Data Studio` to view the SqlServer database data

- Manage DB Schema

1. dotnet tool install --global dotnet-ef
2. dotnet tool update --global dotnet-ef
3. Add Migration: dotnet ef migrations add Initial
4. Remove last Migration: dotnet ef migrations remove
5. Generate SQL script from Migrations: dotnet ef migrations script
6. Update target database: dotnet ef database update
