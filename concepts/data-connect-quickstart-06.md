<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="15a6b-101">Microsoft 365管理员能够批准或拒绝同意请求。</span><span class="sxs-lookup"><span data-stu-id="15a6b-101">A Microsoft 365 administrator has the ability to approve or deny consent requests.</span></span> <span data-ttu-id="15a6b-102">这可以通过管理中心Microsoft 365 PowerShell 以编程方式完成。</span><span class="sxs-lookup"><span data-stu-id="15a6b-102">This can be done via the Microsoft 365 Admin Center or programmatically via PowerShell.</span></span>

## <a name="approve-consent-requests"></a><span data-ttu-id="15a6b-103">批准同意请求</span><span class="sxs-lookup"><span data-stu-id="15a6b-103">Approve consent requests</span></span>

# <a name="microsoft-365-admin-center"></a>[<span data-ttu-id="15a6b-104">Microsoft 365管理中心</span><span class="sxs-lookup"><span data-stu-id="15a6b-104">Microsoft 365 Admin Center</span></span>](#tab/Microsoft365)

1. <span data-ttu-id="15a6b-105">打开浏览器，然后转到你的Microsoft 365[门户。](https://admin.microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="15a6b-105">Open a browser and go to your [Microsoft 365 Admin Portal](https://admin.microsoft.com).</span></span>

1. <span data-ttu-id="15a6b-106">若要批准或拒绝同意请求，请转到 [Privileged Access](https://portal.office.com/adminportal/home#/Settings/PrivilegedAccess)。</span><span class="sxs-lookup"><span data-stu-id="15a6b-106">To approve or deny consent requests, go to [Privileged Access](https://portal.office.com/adminportal/home#/Settings/PrivilegedAccess).</span></span>

1. <span data-ttu-id="15a6b-107">选择一个挂起 **的数据访问请求**。</span><span class="sxs-lookup"><span data-stu-id="15a6b-107">Select a pending **Data Access Request**.</span></span>

1. <span data-ttu-id="15a6b-108">在" **数据访问请求"** 调用中，选择"批准 **"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="15a6b-108">In the **Data Access Request** call out, select the **Approve** button.</span></span>

    ![Screenshot showing a data access request pending consent approval in the Microsoft 365 admin center.](images/data-connect-m365-approve.png)

# <a name="powershell"></a>[<span data-ttu-id="15a6b-110">PowerShell</span><span class="sxs-lookup"><span data-stu-id="15a6b-110">PowerShell</span></span>](#tab/PowerShell)

1. <span data-ttu-id="15a6b-111">打开 Windows PowerShell。</span><span class="sxs-lookup"><span data-stu-id="15a6b-111">Open Windows PowerShell.</span></span>
1. <span data-ttu-id="15a6b-112">确保 PowerShell 会话已启用远程签名的脚本。</span><span class="sxs-lookup"><span data-stu-id="15a6b-112">Ensure that your PowerShell session has enabled remotely signed scripts.</span></span>

    ```powershell
    Set-ExecutionPolicy RemoteSigned
    ```

1. <span data-ttu-id="15a6b-113">连接Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="15a6b-113">Connect to Exchange Online.</span></span>

    1. <span data-ttu-id="15a6b-114">通过执行以下 PowerShell 获取登录凭据。</span><span class="sxs-lookup"><span data-stu-id="15a6b-114">Obtain a sign in credential by executing the following PowerShell.</span></span> <span data-ttu-id="15a6b-115">使用创建和启动 Azure 数据工厂管道的用户登录，该用户应用了全局管理员角色，是拥有批准 Microsoft 365 中数据请求的组的成员，并且启用了多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="15a6b-115">Sign in using a different user than one that created and started the Azure Data Factory pipeline, who has the **Global administrator** role applied, who is a member of the group that has rights to approve requests to data in Microsoft 365, and has multi-factor authentication enabled.</span></span>

        ```powershell
        $UserCredential = Get-Credential
        ```

    1. <span data-ttu-id="15a6b-116">创建新的 PowerShell Exchange Online并加载 (导入) 。</span><span class="sxs-lookup"><span data-stu-id="15a6b-116">Create a new Exchange Online PowerShell session and load (import) it.</span></span>

        ```powershell
        $Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://ps.protection.outlook.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection
        Import-PSSession $Session -DisableNameChecking
        ```

        > [!IMPORTANT]
        > <span data-ttu-id="15a6b-117">完成此会话后，请确保使用 PowerShell 命令断开与会话的连接 `Remove-PSSession $Session` 。</span><span class="sxs-lookup"><span data-stu-id="15a6b-117">After you are finished with this session, be sure you you disconnect from the session using the PowerShell command `Remove-PSSession $Session`.</span></span> <span data-ttu-id="15a6b-118">Exchange Online仅允许三个打开的远程 PowerShell 会话，以抵御拒绝服务 (DoS) 攻击。</span><span class="sxs-lookup"><span data-stu-id="15a6b-118">Exchange Online only allows for three open remote PowerShell sessions to protect against denial-of-service (DoS) attacks.</span></span> <span data-ttu-id="15a6b-119">如果您只是关闭 PowerShell 窗口，它将保持连接打开状态。</span><span class="sxs-lookup"><span data-stu-id="15a6b-119">If you simply close the PowerShell window, it will leave the connection open.</span></span>

1. <span data-ttu-id="15a6b-120">通过执行以下 PowerShell 从 Microsoft Graph 数据连接获取所有待处理数据请求的列表。</span><span class="sxs-lookup"><span data-stu-id="15a6b-120">Get a list of all pending data requests from Microsoft Graph data connect by executing the following PowerShell.</span></span>

    ```powershell
    Get-ElevatedAccessRequest | where {$_.RequestStatus -eq 'Pending'} | select RequestorUPN, Service, Identity, RequestedAccess | fl
    ```

    - <span data-ttu-id="15a6b-121">检查返回的数据访问请求列表。</span><span class="sxs-lookup"><span data-stu-id="15a6b-121">Examine the list of data access requests returned.</span></span> <span data-ttu-id="15a6b-122">在下图中，请注意有两个挂起的请求。</span><span class="sxs-lookup"><span data-stu-id="15a6b-122">In the following image, notice there are two pending requests.</span></span>

        ![Screenshot showing a list of pending requests formatted as a list in a PowerShell console.](images/data-connect-ps-pending-requests.png)

1. <span data-ttu-id="15a6b-124">通过执行以下 PowerShell 复制请求的 Identity GUID，批准在上一步中返回的数据访问。</span><span class="sxs-lookup"><span data-stu-id="15a6b-124">Approve a data access returned in the previous step by copying the Identity GUID of a request by executing the following PowerShell.</span></span>

    > [!NOTE]
    > <span data-ttu-id="15a6b-125">将以下代码段中的 GUID 替换为上一步结果中的 GUID。</span><span class="sxs-lookup"><span data-stu-id="15a6b-125">Replace the GUID in the following code snippet with the GUID from the results of the previous step.</span></span>

    ```powershell
    Approve-ElevatedAccessRequest -RequestId fa041379-0000-0000-0000-7cd5691484bd -Comment 'approval request granted'
    ```

1. <span data-ttu-id="15a6b-126">片刻后，应看到活动运行更新的状态页，以显示它现在 _正在提取数据_。</span><span class="sxs-lookup"><span data-stu-id="15a6b-126">After a few moments, you should see the status page for the activity run update to show it is now _extracting data_.</span></span>

    ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图，其中加载状态现在显示为"正在提取数据"。](images/data-connect-adf-extraction-approved.png)

1. <span data-ttu-id="15a6b-128">提取数据的这一过程可能需要一些时间，具体取决于你的租户Microsoft 365大小。</span><span class="sxs-lookup"><span data-stu-id="15a6b-128">This process of extracting the data can take some time depending on the size of your Microsoft 365 tenant.</span></span>

---

## <a name="verify-extracted-data-from-microsoft-365-to-azure-storage-blob"></a><span data-ttu-id="15a6b-129">验证从数据提取的数据Microsoft 365到Azure 存储 Blob</span><span class="sxs-lookup"><span data-stu-id="15a6b-129">Verify extracted data from Microsoft 365 to Azure Storage Blob</span></span>

1. <span data-ttu-id="15a6b-130">打开浏览器并转到 Azure [门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="15a6b-130">Open a browser and go to your [Azure Portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="15a6b-131">使用具有 Azure 和租户 **全局** 管理员权限Microsoft 365登录。</span><span class="sxs-lookup"><span data-stu-id="15a6b-131">Sign in using an account with **Global administrator** rights to your Azure and Microsoft 365 tenants.</span></span>

1. <span data-ttu-id="15a6b-132">在边栏导航上，选择 **"所有资源"** 菜单项。</span><span class="sxs-lookup"><span data-stu-id="15a6b-132">On the sidebar navigation, select the **All resources** menu item.</span></span>

1. <span data-ttu-id="15a6b-133">在资源列表中，选择 **Azure 存储** 之前在本教程中创建的帐户。</span><span class="sxs-lookup"><span data-stu-id="15a6b-133">In the list of resources, select the **Azure Storage account** you created previously in this tutorial.</span></span>

1. <span data-ttu-id="15a6b-134">在边栏导航菜单上 **，从"** 帐户"边栏选项卡Azure 存储 **Blob"。**</span><span class="sxs-lookup"><span data-stu-id="15a6b-134">On the sidebar navigation menu, select **Blobs** from the **Azure Storage account** blade.</span></span>

1. <span data-ttu-id="15a6b-135">选择 **之前** 在本教程中创建的容器，该容器将 Azure 数据工厂管道配置为提取数据的接收器。</span><span class="sxs-lookup"><span data-stu-id="15a6b-135">Select the **container** created previously in this tutorial that you configured the Azure Data Factory pipeline as the sink for the extracted data.</span></span> <span data-ttu-id="15a6b-136">现在应该会看到此容器中的数据。</span><span class="sxs-lookup"><span data-stu-id="15a6b-136">You should see data in this container now.</span></span>

    ![显示用于帐户服务的 Azure 门户 UI 存储屏幕截图。](images/data-connect-adf-extracted-data-in-blob.png)
