<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="b92c7-101">完成所有先决条件后，你将能够在 Azure AD 管理中心注册应用程序。</span><span class="sxs-lookup"><span data-stu-id="b92c7-101">After all the prerequisites are in place, you will be able to register an application in the Azure AD admin center.</span></span> <span data-ttu-id="b92c7-102">注册是必需的，以便对应用程序进行身份验证，并使用它调用 Microsoft Graph连接器 API。</span><span class="sxs-lookup"><span data-stu-id="b92c7-102">The registration is necessary in order to authenticate the application and use it to make calls to the Microsoft Graph connectors API.</span></span>

1. <span data-ttu-id="b92c7-103">转到管理[Azure Active Directory，](https://aad.portal.azure.com/)然后使用管理员帐户登录。</span><span class="sxs-lookup"><span data-stu-id="b92c7-103">Go to the [Azure Active Directory admin center](https://aad.portal.azure.com/) and sign in with an administrator account.</span></span>
2. <span data-ttu-id="b92c7-104">在左侧窗格中，选择 **"Azure Active Directory"，\*\*\*\*在**"管理"下，选择 **"应用注册"。**</span><span class="sxs-lookup"><span data-stu-id="b92c7-104">On the left pane, select **Azure Active Directory**, and under **Manage**, select **App registrations**.</span></span>
3. <span data-ttu-id="b92c7-105">选择“新注册”。</span><span class="sxs-lookup"><span data-stu-id="b92c7-105">Select **New registration**.</span></span>

    ![显示"应用注册"部分屏幕截图](images/connectors-images/build2.png)

4. <span data-ttu-id="b92c7-107">使用下列 **值填写"注册** 应用程序表单"，然后选择"注册 **"。**</span><span class="sxs-lookup"><span data-stu-id="b92c7-107">Complete the **Register an application** form with the following values, then select **Register**.</span></span>

    <span data-ttu-id="b92c7-108">a.</span><span class="sxs-lookup"><span data-stu-id="b92c7-108">a.</span></span> <span data-ttu-id="b92c7-109">**名称**：部件库存连接器</span><span class="sxs-lookup"><span data-stu-id="b92c7-109">**Name**: Parts Inventory Connector</span></span>

    <span data-ttu-id="b92c7-110">b.</span><span class="sxs-lookup"><span data-stu-id="b92c7-110">b.</span></span> <span data-ttu-id="b92c7-111">**支持的帐户类型**：此组织目录中的帐户仅 (Microsoft - 单租户) </span><span class="sxs-lookup"><span data-stu-id="b92c7-111">**Supported account types**: Accounts in this organizational directory only (Microsoft only - Single tenant)</span></span>

    <span data-ttu-id="b92c7-112">c.</span><span class="sxs-lookup"><span data-stu-id="b92c7-112">c.</span></span> <span data-ttu-id="b92c7-113">**重定向 URI：** 保留为空</span><span class="sxs-lookup"><span data-stu-id="b92c7-113">**Redirect URI**: Leave blank</span></span>

    ![显示"注册应用程序"部分屏幕截图](images/connectors-images/build3-contoso-register-app.png)

5. <span data-ttu-id="b92c7-115">在"部件清单连接器概述"页上，复制"应用程序 (客户端) ID"和" (目录) **ID"的值**。</span><span class="sxs-lookup"><span data-stu-id="b92c7-115">On the Parts Inventory Connector overview page, copy the values of **Application (client) ID and Directory (tenant) ID**.</span></span> <span data-ttu-id="b92c7-116">你将需要在下一节中同时使用这两者。</span><span class="sxs-lookup"><span data-stu-id="b92c7-116">You will need both in the following section.</span></span>

    ![显示"部件清单连接器"部分的屏幕截图](images/connectors-images/build3-contoso-partsinv.png)

6. <span data-ttu-id="b92c7-118">选择 **"管理"下的"API** **权限"。**</span><span class="sxs-lookup"><span data-stu-id="b92c7-118">Select **API Permissions** under **Manage**.</span></span>
7. <span data-ttu-id="b92c7-119">选择 **"添加权限"，** 然后选择 **"Microsoft Graph"。**</span><span class="sxs-lookup"><span data-stu-id="b92c7-119">Select **Add a permission**, then select **Microsoft Graph**.</span></span>
8. <span data-ttu-id="b92c7-120">选择 **"应用程序权限"，** 然后选择 **"ExternalItem.ReadWrite.All"** 权限。</span><span class="sxs-lookup"><span data-stu-id="b92c7-120">Select **Application permissions**, then select the **ExternalItem.ReadWrite.All** permission.</span></span> <span data-ttu-id="b92c7-121">选择 **添加权限**。</span><span class="sxs-lookup"><span data-stu-id="b92c7-121">Select **Add permissions**.</span></span>

    ![显示"请求 API 权限"部分屏幕截图](images/connectors-images/build4.png)

9. <span data-ttu-id="b92c7-123">选择 **"授予 {TENANT} 的管理员同意"，** 然后在 **系统提示时** 选择"是"。</span><span class="sxs-lookup"><span data-stu-id="b92c7-123">Select **Grant admin consent for {TENANT},** then select **Yes** when prompted.</span></span>

    ![显示"部件清单连接器 api 权限"部分的屏幕截图](images/connectors-images/build5.png)

10. <span data-ttu-id="b92c7-125">选择 **"管理 &amp; "下的**"证书 **密码"，** 然后选择"**新建客户端密码"。**</span><span class="sxs-lookup"><span data-stu-id="b92c7-125">Select **Certificates &amp; secrets** under **Manage** , then select **New client secret**.</span></span>
11. <span data-ttu-id="b92c7-126">输入说明并选择密码的过期时间，然后选择"添加 **"。**</span><span class="sxs-lookup"><span data-stu-id="b92c7-126">Enter a description and choose an expiration time for the secret, then select **Add**.</span></span>

    ![显示"部件清单连接器证书和密码"部分的屏幕截图](images/connectors-images/build6.png)

12. <span data-ttu-id="b92c7-128">复制并保存新密码，你将在下面的部分中需要它。</span><span class="sxs-lookup"><span data-stu-id="b92c7-128">Copy and save the new secret, you will need it in the following section.</span></span>
