# mysqlapi

MySQL operations with URL. Based on [data-api-dot-net](https://github.com/mevdschee/data-api-dot-net)

## Get record by id

http://localhost:55263/api.ashx/tableName/Id

**Get record by Id on AspNetUsers table**
```
http://localhost:55263/api.ashx/AspNetUsers/2ee81e34-a384-45d6-8fb2-c370877393a8
```

**returns row in JSON format**
```
{"Id":"2ee81e34-a384-45d6-8fb2-c370877393a8","Email":"ok3@ok.com","EmailConfirmed":false,"PasswordHash":"ACNEtVaVohQFc7wWntjudwCY2mWUWce4ow3g3r9FrulnVJe1HkuTKv8msZpF45md2Q==","SecurityStamp":"8a48cef0-a7e4-47f1-a597-572b4cbdabd0","PhoneNumber":null,"PhoneNumberConfirmed":false,"TwoFactorEnabled":false,"LockoutEndDateUtc":null,"LockoutEnabled":false,"AccessFailedCount":0,"UserName":"ok3@ok.com","ConcurrencyStamp":null,"NormalizedEmail":null,"NormalizedUserName":null}
```

- Tested on Windows
- Dotnet framework 4.5
- Other functions not tested yet
- DB connection info is in api_complex.cs
