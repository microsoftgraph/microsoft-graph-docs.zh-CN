<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="cb183-101">在首次使用 Microsoft Graph Data 连接 之前，需要配置 Microsoft 365 租户。</span><span class="sxs-lookup"><span data-stu-id="cb183-101">Prior to using Microsoft Graph Data Connect for the first time, you need to configure your Microsoft 365 tenant.</span></span> <span data-ttu-id="cb183-102">这涉及打开服务并配置具有批准数据提取请求的权限的安全组。</span><span class="sxs-lookup"><span data-stu-id="cb183-102">This involves turning on the service and configuring a security group with permissions to approve data extraction requests.</span></span>

## <a name="grant-azure-ad-users-the-global-administrator-role"></a><span data-ttu-id="cb183-103">向 Azure AD 用户授予全局管理员角色</span><span class="sxs-lookup"><span data-stu-id="cb183-103">Grant Azure AD users the Global administrator role</span></span>

<span data-ttu-id="cb183-104">在此步骤中，将确保租户中的两Microsoft 365已启用 **全局管理员** 角色。</span><span class="sxs-lookup"><span data-stu-id="cb183-104">In this step, you will ensure that two users in your Microsoft 365 tenant have the **Global administrator** role enabled.</span></span>

- <span data-ttu-id="cb183-105">[全局管理员内置角色](/azure/active-directory/roles/permissions-reference#global-administrator)。</span><span class="sxs-lookup"><span data-stu-id="cb183-105">[Global Administrator built-in role](/azure/active-directory/roles/permissions-reference#global-administrator).</span></span>
- <span data-ttu-id="cb183-106">[提升访问权限以获得全局管理员角色](/azure/role-based-access-control/elevate-access-global-admin)。</span><span class="sxs-lookup"><span data-stu-id="cb183-106">[Elevate access to gain the Global Administrator role](/azure/role-based-access-control/elevate-access-global-admin).</span></span>

## <a name="configure-microsoft-graph-data-connect-consent-request-approver-group"></a><span data-ttu-id="cb183-107">配置 Microsoft Graph数据连接同意请求审批者组</span><span class="sxs-lookup"><span data-stu-id="cb183-107">Configure Microsoft Graph Data Connect consent request approver group</span></span>

<span data-ttu-id="cb183-108">在此步骤中，你将设置你的 Microsoft 365 租户，以允许使用 Microsoft Graph Data 连接。</span><span class="sxs-lookup"><span data-stu-id="cb183-108">In this step, you will setup your Microsoft 365 tenant to enable usage of Microsoft Graph Data Connect.</span></span>

1. <span data-ttu-id="cb183-109">打开浏览器，然后转到你的Microsoft 365[门户。](https://admin.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="cb183-109">Open a browser and go to your [Microsoft 365 Admin Portal](https://admin.microsoft.com/).</span></span>

1. <span data-ttu-id="cb183-110">在边栏导航上，选择"**活动组"。**</span><span class="sxs-lookup"><span data-stu-id="cb183-110">On the sidebar navigation, select **Active Groups**.</span></span>
  
    ![显示管理中心的活动Microsoft 365屏幕截图。](images/data-connect-m365-act-grp.png)

1. <span data-ttu-id="cb183-112">选择" **添加组"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="cb183-112">Select the **Add a group** button.</span></span>

1. <span data-ttu-id="cb183-113">使用以下方法创建新的启用邮件的安全组，然后选择"**添加"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="cb183-113">Use the following to create the new **mail-enabled** security group and select the **Add** button.</span></span>
   - <span data-ttu-id="cb183-114">**类型**：启用邮件的安全性</span><span class="sxs-lookup"><span data-stu-id="cb183-114">**Type**: Mail-enabled security</span></span>

    ![Screenshot showing a user selecting the mail-enabled security for a new group in the Microsoft 365 admin center.](images/data-connect-m365-mail-sec.png)

   - <span data-ttu-id="cb183-116">**名称**：同意请求审批者</span><span class="sxs-lookup"><span data-stu-id="cb183-116">**Name**: Consent Request Approvers</span></span>

    ![显示用户正在管理中心为组提供"同意请求审批者"Microsoft 365屏幕截图。](images/data-connect-m365-cons-apprv.png)

   - <span data-ttu-id="cb183-118">**Email Prefix**： consentrequestapprovers</span><span class="sxs-lookup"><span data-stu-id="cb183-118">**Email Prefix**: consentrequestapprovers</span></span>

    ![Screenshot showing a user creating the email address for the previously created group in the Microsoft 365 admin center.](images/data-connect-m365-cons-apprv-pref.png)

1. <span data-ttu-id="cb183-120">**新创建的组** 最多可能需要一个小时才能显示在列表中。</span><span class="sxs-lookup"><span data-stu-id="cb183-120">**It can take up to an hour** before the newly created group shows up in the list.</span></span> <span data-ttu-id="cb183-121">创建组后，选择它。</span><span class="sxs-lookup"><span data-stu-id="cb183-121">When the group has been created, select it.</span></span>

1. <span data-ttu-id="cb183-122">再次转到 **活动组** 选项，然后搜索你刚刚创建的组。</span><span class="sxs-lookup"><span data-stu-id="cb183-122">Go to the **Active groups** option again and search for the group you just created.</span></span>

1. <span data-ttu-id="cb183-123">选择组，在"成员 **"** 选项卡中，选择"**查看所有和管理成员"。**</span><span class="sxs-lookup"><span data-stu-id="cb183-123">Select the group and in the **Members** tab, select **View all and manage members**.</span></span>

1. <span data-ttu-id="cb183-124">将启用全局管理员角色 **的两个用户** 添加到此新组中。</span><span class="sxs-lookup"><span data-stu-id="cb183-124">Add the two users that you enabled the **Global administrator** role to this new group.</span></span>

## <a name="enable-microsoft-graph-data-connect-in-your-microsoft-365-tenant"></a><span data-ttu-id="cb183-125">在 Graph 租户中连接 Microsoft Microsoft 365 Data Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="cb183-125">Enable Microsoft Graph Data Connect in your Microsoft 365 tenant</span></span>

<span data-ttu-id="cb183-126">在此步骤中，你将在 Graph 租户连接 Microsoft Microsoft 365 服务。</span><span class="sxs-lookup"><span data-stu-id="cb183-126">In this step, you will enable the Microsoft Graph Data Connect service on your Microsoft 365 tenant.</span></span>

1. <span data-ttu-id="cb183-127">当你仍登录到管理门户Microsoft 365，选择 **"设置 >""组织设置"** 菜单项。</span><span class="sxs-lookup"><span data-stu-id="cb183-127">While you are still signed in to the Microsoft 365 Admin Portal, select the **Settings > Org settings** menu item.</span></span>

1. <span data-ttu-id="cb183-128">选择 **Microsoft Graph Data 连接** 服务。</span><span class="sxs-lookup"><span data-stu-id="cb183-128">Select the **Microsoft Graph Data Connect** service.</span></span>

    ![显示"组织设置"边栏选项卡中的"服务"的屏幕截图。](images/data-connect-m365-mgdc-toggle.png)

1. <span data-ttu-id="cb183-131">选中显示为整个组织打开或Graph Microsoft 连接"复选框 **以** 启用数据连接。</span><span class="sxs-lookup"><span data-stu-id="cb183-131">Select the checkbox that says **turn Microsoft Graph Data Connect on or off for your entire organization** to enable Data Connect.</span></span>

    ![显示为整个组织启用数据记录功能而必须连接复选框的屏幕截图。](images/data-connect-m365-enable-mgdc-for-org.png)

1. <span data-ttu-id="cb183-133">输入 **同意请求** (或你之前创建的组的名称) 在用户组中做出审批决定，**然后选择保存。** </span><span class="sxs-lookup"><span data-stu-id="cb183-133">Enter **Consent Request Approvers** (or the name of the group you created previously) in the **group of users to make approval decisions** and select **Save**.</span></span>
