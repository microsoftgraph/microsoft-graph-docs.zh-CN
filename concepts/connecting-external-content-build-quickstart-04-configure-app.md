<!-- markdownlint-disable MD002 MD025 MD041 -->

1. <span data-ttu-id="47f4d-101">在 PartsInventoryConnector.csproj 所在的 (CLI) 打开命令行接口。</span><span class="sxs-lookup"><span data-stu-id="47f4d-101">Open your command line interface (CLI) in the directory where PartsInventoryConnector.csproj is located.</span></span>
2. <span data-ttu-id="47f4d-102">运行以下命令以初始化项目的用户密码。</span><span class="sxs-lookup"><span data-stu-id="47f4d-102">Run the following command to initialize the user secrets for the project.</span></span>

    ```dotnetcli
    dotnet user-secrets init
    ```

3. <span data-ttu-id="47f4d-103">运行以下命令，将应用 ID、应用密码和租户 ID 存储在用户密码存储中。</span><span class="sxs-lookup"><span data-stu-id="47f4d-103">Run the following commands to store your app ID, app secret, and tenant ID in the user secret store.</span></span>
  
    ```dotnetcli
      dotnet user-secrets set appId "YOUR_APP_ID_HERE"
      dotnet user-secrets set appSecret "YOUR_APP_SECRET_HERE"
      dotnet user-secrets set tenantId "YOUR_TENANT_ID_HERE"
    ```
