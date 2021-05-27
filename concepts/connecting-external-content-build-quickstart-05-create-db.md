<!-- markdownlint-disable MD002 MD025 MD041 -->

1. 在 PartsInventoryConnector.csproj 所在的 (CLI) 打开命令行接口。
2. 运行以下命令：

  ```dotnetcli
  dotnet ef migrations add InitialCreate
  dotnet ef database update
  ```

> [!NOTE]
> 如果 CSV 文件中架构发生更改，请运行以下命令，将这些更改反映到 SQLite 数据库中。

```dotnetcli
dotnet ef database drop
dotnet ef database update
```
