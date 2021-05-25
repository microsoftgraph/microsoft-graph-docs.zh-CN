<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="68d6e-101">在此练习中，你将创建、运行和批准 Azure 数据工厂管道，以将数据从 Microsoft 365 提取到 Azure 存储 Blob 进行其他处理。</span><span class="sxs-lookup"><span data-stu-id="68d6e-101">In this exercise you will create, run, and approve an Azure Data Factory pipeline to extract data from Microsoft 365 to an Azure Storage Blob for additional processing.</span></span>

## <a name="create-a-microsoft-azure-active-directory-application-registration"></a><span data-ttu-id="68d6e-102">创建Microsoft Azure Active Directory应用程序注册</span><span class="sxs-lookup"><span data-stu-id="68d6e-102">Create a Microsoft Azure Active Directory application registration</span></span>

<span data-ttu-id="68d6e-103">第一步是创建一个 Azure AD 应用程序，该应用程序将用作运行数据提取过程的安全主体。</span><span class="sxs-lookup"><span data-stu-id="68d6e-103">The first step is to create an Azure AD application that will be used as the security principal to run the data extraction process.</span></span>

1. <span data-ttu-id="68d6e-104">打开浏览器并转到 Azure [门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="68d6e-104">Open a browser and go to your [Azure Portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="68d6e-105">使用具有 Azure 和租户 **全局** 管理员权限Microsoft 365登录。</span><span class="sxs-lookup"><span data-stu-id="68d6e-105">Sign in using an account with **Global administrator** rights to your Azure and Microsoft 365 tenants.</span></span>

1. <span data-ttu-id="68d6e-106">在边栏导航上，选择 **Azure Active Directory (** Azure AD) 。</span><span class="sxs-lookup"><span data-stu-id="68d6e-106">On the sidebar navigation, select **Azure Active Directory** (Azure AD).</span></span>

1. <span data-ttu-id="68d6e-107">在"Azure AD 概述"页上，从菜单 **的** " **管理"部分** 选择"应用注册"。</span><span class="sxs-lookup"><span data-stu-id="68d6e-107">On the Azure AD Overview page, select **App registrations** from the **Manage** section of the menu.</span></span>

1. <span data-ttu-id="68d6e-108">选择" **新建注册"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="68d6e-108">Select the **New registration** button.</span></span>

    ![Screenshot showing the App registrations in the Azure Active Directory service in the Azure portal.](images/data-connect-azure-aad-app-reg.png)

1. <span data-ttu-id="68d6e-110">使用以下值创建新的 Azure AD 应用程序，然后选择"注册 **"。**</span><span class="sxs-lookup"><span data-stu-id="68d6e-110">Use the following values to create a new Azure AD application and select **Register**.</span></span>

   - <span data-ttu-id="68d6e-111">**名称**：Microsoft Graph数据连接数据传输</span><span class="sxs-lookup"><span data-stu-id="68d6e-111">**Name**: Microsoft Graph Data Connect Data Transfer</span></span>
   - <span data-ttu-id="68d6e-112">**支持的帐户类型**：仅此组织目录中的帐户。</span><span class="sxs-lookup"><span data-stu-id="68d6e-112">**Supported account types**: Accounts in this organizational directory only.</span></span>
   - <span data-ttu-id="68d6e-113">**重定向 URI：** 保留默认值。</span><span class="sxs-lookup"><span data-stu-id="68d6e-113">**Redirect URI**: Leave the default values.</span></span>

    ![显示在 Azure 门户中注册新应用程序注册的步骤的屏幕截图。](images/data-connect-aad-redirect-uri.png)

1. <span data-ttu-id="68d6e-115">找到 **应用程序 (客户端) ID** 并复制它，因为本教程稍后将对此进行介绍。</span><span class="sxs-lookup"><span data-stu-id="68d6e-115">Locate the **Application (client) ID** and copy it as you will need it later in this tutorial.</span></span> <span data-ttu-id="68d6e-116">这称为服务主体 ID。</span><span class="sxs-lookup"><span data-stu-id="68d6e-116">This will be referred to as the service principal ID.</span></span>

1. <span data-ttu-id="68d6e-117">找到 **目录 (租户) ID，** 并复制它，因为本教程稍后将对此进行介绍。</span><span class="sxs-lookup"><span data-stu-id="68d6e-117">Locate the **Directory (tenant) ID** and copy it as you will need it later in this tutorial.</span></span> <span data-ttu-id="68d6e-118">这称为租户 ID。</span><span class="sxs-lookup"><span data-stu-id="68d6e-118">This will be referred to as the tenant ID.</span></span>

1. <span data-ttu-id="68d6e-119">在边栏导航上，选择"管理 **"下的"证书和\*\*\*\*密码"。**</span><span class="sxs-lookup"><span data-stu-id="68d6e-119">On the sidebar navigation, select **Certificates and secrets** under **Manage**.</span></span>

1. <span data-ttu-id="68d6e-120">选择" **新建客户端密码"按钮**。</span><span class="sxs-lookup"><span data-stu-id="68d6e-120">Select the **New client secret button**.</span></span> <span data-ttu-id="68d6e-121">将 *"说明*"设置为任意名称，将 **"到期**"设置为下拉列表中的任意值，然后选择"添加 **"。**</span><span class="sxs-lookup"><span data-stu-id="68d6e-121">Set *Description* to any name, set **Expires** to any value in the dropdown and choose **Add**.</span></span>

    ![显示在 Azure 门户中创建新客户端密码的过程的屏幕截图。](images/data-connect-aad-certs-secrets.png)

    - <span data-ttu-id="68d6e-123">创建客户端密码后，请确保将 **"** 值"保存在安全位置，因为稍后将不再可用，并且需要创建新的密码。</span><span class="sxs-lookup"><span data-stu-id="68d6e-123">After the client secret is created, make sure you save the **Value** somewhere safe, as it will no longer be available later, and you will need to create a new one.</span></span>
    - <span data-ttu-id="68d6e-124">这将作为服务主体密钥引用。</span><span class="sxs-lookup"><span data-stu-id="68d6e-124">This will be referenced as the service principal key.</span></span>

1. <span data-ttu-id="68d6e-125">在应用程序的边栏导航上，选择"所有者 **"。**</span><span class="sxs-lookup"><span data-stu-id="68d6e-125">On the sidebar navigation for the application, select **Owners**.</span></span>

1. <span data-ttu-id="68d6e-126">验证您的帐户是否列为应用程序的所有者。</span><span class="sxs-lookup"><span data-stu-id="68d6e-126">Verify that your account is listed as an owner for the application.</span></span> <span data-ttu-id="68d6e-127">如果未列为所有者，请添加它。</span><span class="sxs-lookup"><span data-stu-id="68d6e-127">If it isn't listed as an owner, add it.</span></span>

    ![显示用户确认其帐户已设置为 Azure 门户中应用程序注册的所有者的屏幕截图。](images/data-connect-aad-app-owners.png)
