<!-- markdownlint-disable MD002 MD025 MD041 -->

在此步骤中，将生成并运行示例。 此代码示例将创建一个新连接，注册架构，然后将项目从 [ApplianceParts.csv文件推送 ](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/ApplianceParts.csv) 到该连接。

1. 在 PartsInventoryConnector (CLI) 打开命令行接口。
2. 使用 命令： `dotnet build` 生成示例。
3. 使用 命令： `dotnet run` 运行示例。
4. 选择"**1"。创建连接**"。 输入该连接的唯一标识符、名称和说明。
5. 选择 **"2"。为当前连接选项"注册架构**"，然后等待操作完成。
6. 选择 **"3"。将所有项目推送到当前连接**。

  > [!NOTE]
  > 如果步骤 5 导致错误，请等待几分钟，然后选择"**3"。将所有项目推送到当前** 连接"。
