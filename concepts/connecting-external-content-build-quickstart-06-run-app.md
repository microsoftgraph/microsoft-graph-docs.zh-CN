<!-- markdownlint-disable MD002 MD025 MD041 -->

<span data-ttu-id="426b6-101">在此步骤中，将生成并运行示例。</span><span class="sxs-lookup"><span data-stu-id="426b6-101">In this step, you will build and run the sample.</span></span> <span data-ttu-id="426b6-102">此代码示例将创建一个新连接，注册架构，然后将项目从 [ApplianceParts.csv文件推送 ](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/ApplianceParts.csv) 到该连接。</span><span class="sxs-lookup"><span data-stu-id="426b6-102">This code sample will create a new connection, register the schema, then push items from the [ApplianceParts.csv](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/ApplianceParts.csv) file into that connection.</span></span>

1. <span data-ttu-id="426b6-103">在 PartsInventoryConnector (CLI) 打开命令行接口。</span><span class="sxs-lookup"><span data-stu-id="426b6-103">Open your command-line interface (CLI) in the PartsInventoryConnector directory.</span></span>
2. <span data-ttu-id="426b6-104">使用 命令： `dotnet build` 生成示例。</span><span class="sxs-lookup"><span data-stu-id="426b6-104">Use the command: `dotnet build` to build the sample.</span></span>
3. <span data-ttu-id="426b6-105">使用 命令： `dotnet run` 运行示例。</span><span class="sxs-lookup"><span data-stu-id="426b6-105">Use the command: `dotnet run` to run the sample.</span></span>
4. <span data-ttu-id="426b6-106">选择"**1"。创建连接**"。</span><span class="sxs-lookup"><span data-stu-id="426b6-106">Select "**1. Create a connection**".</span></span> <span data-ttu-id="426b6-107">输入该连接的唯一标识符、名称和说明。</span><span class="sxs-lookup"><span data-stu-id="426b6-107">Enter a unique identifier, name, and description for that connection.</span></span>
5. <span data-ttu-id="426b6-108">选择 **"2"。为当前连接选项"注册架构**"，然后等待操作完成。</span><span class="sxs-lookup"><span data-stu-id="426b6-108">Select "**2. Register schema for the current connection option**" Then, wait for the operation to complete.</span></span>

  > [!NOTE]
  > <span data-ttu-id="426b6-109">如果此步骤导致错误，请等待几分钟，然后选择"**3"。将所有项目推送到当前** 连接"。</span><span class="sxs-lookup"><span data-stu-id="426b6-109">If this step results in an error, wait a few minutes, and then select "**3. Push all items to current connection**".</span></span>
