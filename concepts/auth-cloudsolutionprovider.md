---
title: 从云解决方案提供商应用程序中调用 Microsoft Graph
description: 本主题介绍如何使应用程序使用授权代码授予流或服务到服务客户端凭据流，通过 Microsoft Graph 访问合作伙伴托管的客户数据。
author: jackson-woods
localization_priority: Priority
ms.prod: applications
ms.custom: graphiamtop20
ms.openlocfilehash: cb6480bd595684249b8778c3f7200c3b112cbefb
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760817"
---
# <a name="call-microsoft-graph-from-a-cloud-solution-provider-application"></a><span data-ttu-id="22add-103">从云解决方案提供商应用程序中调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="22add-103">Call Microsoft Graph from a Cloud Solution Provider application</span></span>

> <span data-ttu-id="22add-p101">**注意：** 本主题 **仅** 适用于 Microsoft 云解决方案提供商 (CSP) 应用程序开发者。[Microsoft 云解决方案提供商 (CSP)](https://partner.microsoft.com/cloud-solution-provider) 计划使 Microsoft 的合作伙伴可以管理 Microsoft Online Services 并将其转售给客户。</span><span class="sxs-lookup"><span data-stu-id="22add-p101">**Note:** This topic applies **only** to Microsoft Cloud Solution Provider (CSP) application developers. The [Microsoft Cloud Solution Provider (CSP)](https://partner.microsoft.com/cloud-solution-provider) program enables Microsoft’s partners to resell and manage Microsoft Online services to customers.</span></span>

<span data-ttu-id="22add-106">本主题介绍如何使应用程序使用[授权代码授予流](/azure/active-directory/develop/active-directory-protocols-oauth-code)或[服务到服务客户端凭据流](/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service)，通过 Microsoft Graph 访问合作伙伴托管的客户数据。</span><span class="sxs-lookup"><span data-stu-id="22add-106">This topic describes how to enable application access to partner-managed customer data via Microsoft Graph using either the [authorization code grant flow](/azure/active-directory/develop/active-directory-protocols-oauth-code) or the [service to service client credentials flow](/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service).</span></span>

<span data-ttu-id="22add-107">**重要说明：** 从 CSP 应用程序中调用 Microsoft Graph 仅受目录资源（例如 **用户**、**组**、**设备**、**组织**）和 [Intune](/graph/api/resources/intune-graph-overview?view=graph-rest-beta) 资源支持。</span><span class="sxs-lookup"><span data-stu-id="22add-107">**Important:** Calling Microsoft Graph from a CSP application is only supported for directory resources (such as **user**, **group**,**device**, **organization**) and [Intune](/graph/api/resources/intune-graph-overview?view=graph-rest-beta) resources.</span></span>

## <a name="what-is-a-partner-managed-application"></a><span data-ttu-id="22add-108">什么是合作伙伴托管的应用程序</span><span class="sxs-lookup"><span data-stu-id="22add-108">What is a partner-managed application</span></span>

<span data-ttu-id="22add-p102">CSP 计划使 Microsoft 的合作伙伴可以管理 Microsoft Online Services（例如 Microsoft 365、Microsoft Azure 和 CRM Online）并将其转售给客户。客户服务的管理是通过委派管理员特权完成的，这使委派的合作伙伴用户（称为代理）可以访问并配置其客户的环境。</span><span class="sxs-lookup"><span data-stu-id="22add-p102">The CSP program enables Microsoft’s partners to resell and manage Microsoft Online Services (such as Microsoft 365, Microsoft Azure, and CRM Online) to customers. Management of customer services is done through Delegated Admin Privileges, which enables designated partner users (known as agents) to access and configure their customers’ environments.</span></span>

<span data-ttu-id="22add-p103">此外，作为合作伙伴开发者，你可以构建 **合作伙伴托管的应用** 来管理客户的 Microsoft 服务。合作伙伴托管的应用通常称为 *预先同意的* 应用，因为所有客户都已自动预先同意合作伙伴托管的应用。这意味着，当某个客户租户中的用户使用一个合作伙伴托管的应用时，用户不会收到给予同意的提示就能使用该应用。合作伙伴托管的应用还可以继承委派的管理员特权，因此，你的合作伙伴代理还可以通过合作伙伴托管的应用程序获取对客户的特权访问。</span><span class="sxs-lookup"><span data-stu-id="22add-p103">Additionally, as a partner developer, you can build a **partner-managed app** to manage your customers' Microsoft services. Partner-managed apps are often called *pre-consented* apps because all your customers are automatically pre-consented for your partner-managed apps. This means when a user from one of your customer tenants uses one of your partner-managed apps, the user can use it without being prompted to give consent. Partner-managed apps also inherit Delegated Admin Privileges, so your partner agents can also get privileged access to your customers through your partner-managed application.</span></span>

## <a name="how-to-set-up-a-partner-managed-application"></a><span data-ttu-id="22add-115">如何设置合作伙伴托管的应用程序</span><span class="sxs-lookup"><span data-stu-id="22add-115">How to set-up a partner-managed application</span></span>

<span data-ttu-id="22add-116">被授予访问客户数据的提升权限时，应用程序被视为 *合作伙伴托管*。</span><span class="sxs-lookup"><span data-stu-id="22add-116">An application is viewed as *partner-managed* when it is granted elevated permissions to access your customers' data.</span></span>

> <span data-ttu-id="22add-117">**注意：** 合作伙伴托管的应用 *仅* 可以在合作伙伴租户中配置，为管理客户租户资源，合作伙伴托管的应用 **必须** 配置为 **多租户应用程序**。</span><span class="sxs-lookup"><span data-stu-id="22add-117">**Note:** Partner-managed apps can *only* be configured on Partner tenants, and in order to manage customer tenant resources, partner-managed apps **must** be configured as **multi-tenant applications**.</span></span>

### <a name="register-and-configure-a-multi-tenant-app"></a><span data-ttu-id="22add-118">注册和配置多租户应用</span><span class="sxs-lookup"><span data-stu-id="22add-118">Register and configure a multi-tenant app</span></span>

<span data-ttu-id="22add-119">此处所需的初始步骤与注册和配置多租户应用程序所用的步骤相同：</span><span class="sxs-lookup"><span data-stu-id="22add-119">The initial steps required here follow most of the same steps used to register and configure a multi-tenant application:</span></span>

1. <span data-ttu-id="22add-p104">使用 [Azure 门户](https://portal.azure.com)在合作伙伴租户中[注册应用程序](/azure/active-directory/active-directory-app-registration)。若要作为合作伙伴托管的应用，必须将应用程序配置为[多租户应用](/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#update-registration-to-be-multi-tenant)。此外，如果应用已经过部署并在多个地理区域中销售，你将需要如<a href="#region">此处</a>所述在每个区域中注册你的应用。</span><span class="sxs-lookup"><span data-stu-id="22add-p104">[Register your application](/azure/active-directory/active-directory-app-registration) in your Partner tenant using the [Azure Portal](https://portal.azure.com). To function as a partner-managed app, an application must be configured as a [multi-tenant app](/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#update-registration-to-be-multi-tenant). Additionally, if your app is deployed and sold in multiple geographic regions you will need to register your app in each of those regions as described <a href="#region">here</a>.</span></span>
2. <span data-ttu-id="22add-123">使用最低特权的方法，再次通过 Azure 门户为多租户应用配置需要的 *必要权限*。</span><span class="sxs-lookup"><span data-stu-id="22add-123">Configure your multi-tenant app, again through the Azure Portal, with the *required permissions* it needs using a least privileged approach.</span></span>

### <a name="pre-consent-your-app-for-all-your-customers"></a><span data-ttu-id="22add-124">为你的所有客户预先同意应用</span><span class="sxs-lookup"><span data-stu-id="22add-124">Pre-consent your app for all your customers</span></span>

<span data-ttu-id="22add-p105">为你的所有客户最终授予合作伙伴托管的应用的已配置权限。你可以通过使用 Azure AD powershell V2 将代表应用的 **servicePrincipal** 添加到合作伙伴租户中的 *Adminagents* 组，以执行此操作。你可以在 [此处](https://www.powershellgallery.com/packages/AzureAD)下载和安装 Azure AD PowerShell V2。按照以下步骤查找 *Adminagents* 组、**servicePrincipal** 并将其添加到组。</span><span class="sxs-lookup"><span data-stu-id="22add-p105">Finally grant your partner-managed app those configured permissions for all your customers. You can do this by adding the **servicePrincipal** that represents the app to the *Adminagents* group in your Partner tenant, using Azure AD powershell V2. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).  Follow these steps to find the *Adminagents* group, the **servicePrincipal** and add it to the group.</span></span>

1. <span data-ttu-id="22add-129">打开 PowerShell 会话，并通过在登录窗口中输入管理员凭据连接到合作伙伴租户。</span><span class="sxs-lookup"><span data-stu-id="22add-129">Open a PowerShell session and connect to your partner tenant by entering your admin credentials into the sign-in window.</span></span>

    ```PowerShell
    Connect-AzureAd
    ```

2. <span data-ttu-id="22add-130">查找代表 *Adminagents* 的组。</span><span class="sxs-lookup"><span data-stu-id="22add-130">Find the group that represents the *Adminagents*.</span></span>

    ```PowerShell
    $group = Get-AzureADGroup -Filter "displayName eq 'Adminagents'"
    ```

3. <span data-ttu-id="22add-131">查找与应用具有相同 *appId* 的服务主体。</span><span class="sxs-lookup"><span data-stu-id="22add-131">Find the service principal that has the same *appId* as your app.</span></span>

    ```PowerShell
    $sp = Get-AzureADServicePrincipal -Filter "appId eq '{yourAppsAppId}'"
    ```

4. <span data-ttu-id="22add-132">最后，将服务主体添加到 *Adminagents* 组中。</span><span class="sxs-lookup"><span data-stu-id="22add-132">Finally, add the service principal to the *Adminagents* group.</span></span>

    ```PowerShell
    Add-AzureADGroupMember -ObjectId $group.ObjectId -RefObjectId $sp.ObjectId
    ```

## <a name="token-acquisition-flows"></a><span data-ttu-id="22add-133">令牌购置流</span><span class="sxs-lookup"><span data-stu-id="22add-133">Token acquisition flows</span></span>

<span data-ttu-id="22add-134">合作伙伴托管的应用的令牌购置流（[授权代码授予流](/azure/active-directory/develop/active-directory-protocols-oauth-code)和[服务到服务客户端凭据流](/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service)）与常规的多租户应用相同。</span><span class="sxs-lookup"><span data-stu-id="22add-134">Token acquisition flows for partner-managed apps - [authorization code grant flow](/azure/active-directory/develop/active-directory-protocols-oauth-code) and [service-to-service client credentials flow](/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service) - are the same as regular multi-tenant apps.</span></span>

<span data-ttu-id="22add-p106">除了预先同意访问所有客户租户外，合作伙伴托管的应用还具有其他功能。它允许你的代理使用应用访问客户的租户数据（使用委派的管理员特权）。从概念上讲，工作原理如下：</span><span class="sxs-lookup"><span data-stu-id="22add-p106">Apart from pre-consented access to all your customer tenants, partner-managed apps have one additional capability. It allows for your agents to use your app to access your customers' tenant data (using delegated admin privileges). Conceptually it works like this:</span></span>

1. <span data-ttu-id="22add-138">代理使用从合作伙伴租户颁发的用户凭据登录你的应用。</span><span class="sxs-lookup"><span data-stu-id="22add-138">Your agent signs in to your app with their user credentials issued from your partner tenant.</span></span>
2. <span data-ttu-id="22add-139">你的应用请求对目标合作伙伴托管的客户租户的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="22add-139">Your app requests an access token for the intended partner-managed customer tenant.</span></span>
3. <span data-ttu-id="22add-140">你的应用使用访问令牌调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="22add-140">Your app uses the access token to call Microsoft Graph.</span></span>

<span data-ttu-id="22add-p107">除了代理必须使用其合作伙伴帐户登录之外，这是标准的 [授权代码授予流](/azure/active-directory/develop/active-directory-protocols-oauth-code)。若要查看其工作原理，请假设你的合作伙伴租户是 *partner.com*（这是代理的主租户），并将你的一位客户假设为 *customer.com*：</span><span class="sxs-lookup"><span data-stu-id="22add-p107">This is a standard [authorization code grant flow](/azure/active-directory/develop/active-directory-protocols-oauth-code), except that your agents must sign-in using their partner accounts. To see how this would look, imagine your partner tenant is *partner.com* (which is the home tenant for your agents) and one of your customers is *customer.com*:</span></span>

1. <span data-ttu-id="22add-p108">[获取授权代码：](/azure/active-directory/develop/active-directory-protocols-oauth-code#request-an-authorization-code)在我们的示例 ```customer.com``` 中，对于目标租户，你的应用会对 ```/authorize``` 终结点发出请求，且必须使用 **客户租户** 你的代理将仍然使用其 ```username@partner.com``` 帐户登录。</span><span class="sxs-lookup"><span data-stu-id="22add-p108">[Acquire an authorization code:](/azure/active-directory/develop/active-directory-protocols-oauth-code#request-an-authorization-code) Your app makes a request to the ```/authorize``` endpoint and must use a **customer tenant**, in our example ```customer.com```, for the target tenant. Your agents would still sign-in with their ```username@partner.com``` account.</span></span>

    ```http
    GET https://login.microsoftonline.com/customer.com/oauth2/authorize
    ```

2. <span data-ttu-id="22add-145">[使用授权代码获取访问令牌：](/azure/active-directory/develop/active-directory-protocols-oauth-code#use-the-authorization-code-to-request-an-access-token)在我们的示例 ```customer.com``` 中，当对 ```token``` 终结点发出请求时，你的应用必须将 **客户租户** 用作目标租户：</span><span class="sxs-lookup"><span data-stu-id="22add-145">[Acquire an access token using the authorization code:](/azure/active-directory/develop/active-directory-protocols-oauth-code#use-the-authorization-code-to-request-an-access-token) Your app must use a **customer tenant** as the target tenant, in our example ```customer.com```, when making the request to the ```token``` endpoint:</span></span>

    ```http
    POST https://login.microsoftonline.com/customer.com/oauth2/token
    ```

3. <span data-ttu-id="22add-146">现在你拥有了访问令牌，请调用 Microsoft Graph，将访问令牌置于 HTTP 授权标头中：</span><span class="sxs-lookup"><span data-stu-id="22add-146">Now you have an access token, call Microsoft Graph, putting the access token in the HTTP authorization header:</span></span>

    ```http
    GET https://graph.microsoft.com/beta/users
    Authorization: Bearer <token>
    ```

## <a name="register-your-app-in-the-regions-you-support"></a><span data-ttu-id="22add-147">在支持的区域中注册你的应用</span><span class="sxs-lookup"><span data-stu-id="22add-147">Register your app in the regions you support</span></span>
<a name="region"></a>

<span data-ttu-id="22add-p109">CSP 客户服务当前仅限于单个区域。合作伙伴托管的应用程序执行相同的限制。这意味着你在进行销售的每个区域必须具有单独的租户。例如，如果合作伙伴托管的应用在位于美国的租户中注册，但你的客户位于英国，合作伙伴托管的应用将无法工作。每个区域合作伙伴租户必须维护自己的一组合作伙伴托管的应用，才能管理相同区域内的客户。这可能需要应用中的其他逻辑（登录前）获取用户的登录用户名，才能决定使用哪个特定于区域的合作伙伴托管的标识来为用户提供服务。</span><span class="sxs-lookup"><span data-stu-id="22add-p109">CSP customer engagement is currently limited to a single region. Partner-managed applications carry the same limitation. This means you must have a separate tenant for each region you sell in. For example, if your partner-managed app is registered in a tenant in the US but your customer is in the EU – the partner-managed app will not work.  Each of your regional partner tenants must maintain their own set of partner-managed apps to manage customers within the same region. This might require additional logic in your app (prior to sign-in) to get your customers' sign-in username to decide which region-specific partner-managed app identity to use, to serve the user.</span></span>

## <a name="calling-microsoft-graph-immediately-after-customer-creation"></a><span data-ttu-id="22add-154">创建客户后立即调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="22add-154">Calling Microsoft Graph immediately after customer creation</span></span>

<span data-ttu-id="22add-p110">使用[合作伙伴中心 API](https://partnercenter.microsoft.com/partner/developer) 创建新客户时会创建新的客户租户。此外，还会创建合作伙伴关系，这使你成为此新客户租户的在案合作伙伴。这种伙伴关系可能需要最多 3 分钟传播给新客户租户。如果应用在创建后直接调用 Microsoft Graph，应用可能会接收拒绝访问错误。当现有客户接受你的邀请时可能会遇到类似延迟。这是因为预先同意依赖于客户租户中现已存在的合作伙伴关系。</span><span class="sxs-lookup"><span data-stu-id="22add-p110">When you create a new customer using the [Partner Center API](https://partnercenter.microsoft.com/partner/developer), a new customer tenant gets created. Additionally, a partner relationship also gets created, which makes you the partner of record for this new customer tenant. This partner relationship can take up to 3 minutes to propagate to the new customer tenant. If your app calls Microsoft Graph straight after creation, your app will likely receive an access denied error. A similar delay may be experienced when an existing customer accepts your invitation. This is because pre-consent relies on the partner relationship being present in the customer tenant.</span></span>

<span data-ttu-id="22add-161">为避免此问题，在调用 Azure AD 以获取令牌（从而调用 Microsoft Graph）之前，我们建议你的合作伙伴应用应在创建客户后等待 **三分钟**。</span><span class="sxs-lookup"><span data-stu-id="22add-161">To avoid this problem, we recommend that your partner app should wait **three minutes** after customer creation before calling Azure AD to acquire a token (to call Microsoft Graph).</span></span> <span data-ttu-id="22add-162">这应该涵盖了大多数情况。</span><span class="sxs-lookup"><span data-stu-id="22add-162">This should cover most cases.</span></span> <span data-ttu-id="22add-163">但是，如果等待三分钟后仍收到授权错误，请再等待 60 秒后重试。</span><span class="sxs-lookup"><span data-stu-id="22add-163">However, if after waiting three minutes you still receive an authorization error, please wait an additional 60 seconds and try again.</span></span>

> <span data-ttu-id="22add-p112">**注意：** 重试时，你必须在调用 Microsoft Graph 之前从 Azure AD 获取新的访问令牌。你将无法使用已经拥有的访问令牌调用 Microsoft Graph，因为访问令牌只能使用一小时，且不包含预先同意的权限声明。</span><span class="sxs-lookup"><span data-stu-id="22add-p112">**Note:** On the retry, you must acquire a new access token from Azure AD, before calling Microsoft Graph.  Calling Microsoft Graph with the access token you already have will not work, because the access token is good for an hour and won’t contain the pre-consented permission claims.</span></span>