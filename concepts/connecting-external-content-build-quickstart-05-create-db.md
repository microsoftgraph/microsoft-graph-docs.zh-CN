<!-- markdownlint-disable MD002 MD025 MD041 -->

1. <span data-ttu-id="39b41-101">在 PartsInventoryConnector.csproj 所在的 (CLI) 打开命令行接口。</span><span class="sxs-lookup"><span data-stu-id="39b41-101">Open your command line interface (CLI) in the directory where PartsInventoryConnector.csproj is located.</span></span>
2. <span data-ttu-id="39b41-102">运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="39b41-102">Run the following commands:</span></span>

  ```dotnetcli
  dotnet ef migrations add InitialCreate
  dotnet ef database update
  ```

> [!NOTE]
> <span data-ttu-id="39b41-103">如果 CSV 文件中架构发生更改，请运行以下命令，将这些更改反映到 SQLite 数据库中。</span><span class="sxs-lookup"><span data-stu-id="39b41-103">Run the following commands if a schema changes in the CSV file, and reflect those changes into the SQLite database.</span></span>

```dotnetcli
dotnet ef database drop
dotnet ef database update
```
