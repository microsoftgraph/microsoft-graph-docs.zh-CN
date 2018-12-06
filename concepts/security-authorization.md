---
title: 授权和 Microsoft Graph 安全 API
description: 敏感并受权限和 Azure Active Directory (Azure AD) 角色，可通过 Microsoft Graph 安全 API 访问的安全数据。
ms.openlocfilehash: c69621fa7059a96381bed76b58c4a77e80d984dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091741"
---
# <a name="authorization-and-the-microsoft-graph-security-api"></a><span data-ttu-id="3e4e5-103">授权和 Microsoft Graph 安全 API</span><span class="sxs-lookup"><span data-stu-id="3e4e5-103">Authorization and the Microsoft Graph Security API</span></span>

<span data-ttu-id="3e4e5-104">敏感并受权限和 Azure Active Directory (Azure AD) 角色，可通过 Microsoft Graph 安全 API 访问的安全数据。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-104">Security data accessible via the Microsoft Graph Security API is sensitive and protected by both permissions and Azure Active Directory (Azure AD) roles.</span></span>

<span data-ttu-id="3e4e5-105">Microsoft Graph 安全 API 支持两种类型的授权：</span><span class="sxs-lookup"><span data-stu-id="3e4e5-105">The Microsoft Graph Security API supports two types of authorization:</span></span>

- <span data-ttu-id="3e4e5-106">**应用程序级别授权** - 没有已登录的用户（例如，SIEM 应用场景）。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-106">**Application-level authorization** - There is no signed-in user (for example, a SIEM scenario).</span></span> <span data-ttu-id="3e4e5-107">授权由授予给应用程序的权限决定。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-107">The permissions granted to the application determine authorization.</span></span> 
    ><span data-ttu-id="3e4e5-108">**注意：** 此选项还可以支持基于角色的访问控制 (RBAC) 由应用程序管理的情况。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-108">**Note:** This option can also support cases where Role-Based Access Control (RBAC) is managed by the application.</span></span>
- <span data-ttu-id="3e4e5-109">**用户委派授权** - 身份为 Azure AD 租户成员的用户已登录。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-109">**User delegated authorization** - A user who is a member of the Azure AD tenant is signed in.</span></span> <span data-ttu-id="3e4e5-110">除了已被授予所需权限的应用程序之外，用户必须是 Azure AD 有限管理员角色的成员 - 安全读者或安全管理员。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-110">The user must be a member of an Azure AD Limited Admin role - either Security Reader or Securty Administrator - in addition to the application having been granted the required permissions.</span></span>

<span data-ttu-id="3e4e5-111">如果您从图资源管理器呼叫 Microsoft Graph 安全 API:</span><span class="sxs-lookup"><span data-stu-id="3e4e5-111">If you're calling the Microsoft Graph Security API from Graph Explorer:</span></span>

- <span data-ttu-id="3e4e5-112">Azure AD 租户管理员必须对 Graph 浏览器应用程序显式授予所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-112">The Azure AD tenant admin must explicitly grant consent for the requested permissions to the Graph Explorer application.</span></span>
- <span data-ttu-id="3e4e5-113">用户必须是 Azure AD 中安全读者有限管理员角色的成员（安全读者或安全管理员）。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-113">The user must be a member of the Security Reader Limited Admin role in Azure AD (either Security Reader or Security Administrator).</span></span>

><span data-ttu-id="3e4e5-114">**注意**：Graph 浏览器不支持应用程序级别授权。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-114">**Note**: Graph Explorer does not support application-level authorization.</span></span>

<span data-ttu-id="3e4e5-115">如果您正在从自定义或自己的应用程序中调用 Microsoft Graph 安全 API:</span><span class="sxs-lookup"><span data-stu-id="3e4e5-115">If you're calling the Microsoft Graph Security API from a custom or your own application:</span></span>

- <span data-ttu-id="3e4e5-116">Azure AD 租户管理员必须对你的应用程序显式授权。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-116">The Azure AD tenant admin must explicitly grant consent to your application.</span></span> <span data-ttu-id="3e4e5-117">这对于应用程序级别授权和用户委派授权都是必需的。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-117">This is required both for application-level authorization and user delegated authorization.</span></span>
- <span data-ttu-id="3e4e5-118">如果正在使用用户委派授权，用户必须是 Azure AD 中安全读者或安全管理员有限管理员角色的成员。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-118">If you're using user delegated authorization, the user must be a member of the Security Reader or Security Administrator Limited Admin role in Azure AD.</span></span>

## <a name="manage-authorization-in-security-api-client-applications"></a><span data-ttu-id="3e4e5-119">管理安全 API 客户端应用程序中的授权</span><span class="sxs-lookup"><span data-stu-id="3e4e5-119">Manage authorization in security API client applications</span></span>

<span data-ttu-id="3e4e5-120">通过 Microsoft Graph 安全 API 所提供的安全数据写，必须受适当的身份验证和授权机制。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-120">Security data provided via the Microsoft Graph Security API is sensitive and must be protected by appropriate authentication and authorization mechanisms.</span></span> <span data-ttu-id="3e4e5-121">下表列出了注册和创建可以访问 Microsoft Graph 安全 API 的客户端应用程序的步骤。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-121">The following table lists the steps to register and create a client application that can access the Microsoft Graph Security API.</span></span>

| <span data-ttu-id="3e4e5-122">**谁**</span><span class="sxs-lookup"><span data-stu-id="3e4e5-122">**Who**</span></span> | <span data-ttu-id="3e4e5-123">**操作**</span><span class="sxs-lookup"><span data-stu-id="3e4e5-123">**Action**</span></span> |
|:---------------------|:------------------|
|<span data-ttu-id="3e4e5-124">应用程序开发人员或所有者：</span><span class="sxs-lookup"><span data-stu-id="3e4e5-124">Application developer or owner</span></span>|<span data-ttu-id="3e4e5-125">将应用程序注册为企业应用程序。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-125">Register the application as an enterprise application.</span></span>|
|<span data-ttu-id="3e4e5-126">租户管理员</span><span class="sxs-lookup"><span data-stu-id="3e4e5-126">Tenant admin</span></span>|<span data-ttu-id="3e4e5-127">向应用程序授予权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-127">Grant permissions to the application.</span></span>|
|<span data-ttu-id="3e4e5-128">租户管理员</span><span class="sxs-lookup"><span data-stu-id="3e4e5-128">Tenant admin</span></span>|<span data-ttu-id="3e4e5-129">为用户分配角色。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-129">Assign roles to users.</span></span>|
|<span data-ttu-id="3e4e5-130">应用程序开发人员</span><span class="sxs-lookup"><span data-stu-id="3e4e5-130">Application developer</span></span>|<span data-ttu-id="3e4e5-131">用户登录并使用应用程序访问 Microsoft Graph 安全 API。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-131">Sign in as the user and use the application to access the Microsoft Graph Security API.</span></span>|

<span data-ttu-id="3e4e5-132">应用程序注册仅定义应用程序运行所需的权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-132">Application registration only defines which permissions the application needs in order to run.</span></span> <span data-ttu-id="3e4e5-133">它不对应用程序进行这些权限的授予。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-133">It does NOT grant these permissions to the application.</span></span>

<span data-ttu-id="3e4e5-134">Azure AD 租户管理员必须对应用程序显式授予权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-134">The Azure AD tenant administrator MUST explicitly grant the permissions to the application.</span></span> <span data-ttu-id="3e4e5-135">这必须按每租户实施，并且必须在应用程序权限在应用程序注册门户中*每次更改时执行*。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-135">This must be done per tenant and must be *performed every time* the application permissions are changed in the application registration portal.</span></span>

<span data-ttu-id="3e4e5-136">例如，假定你拥有一个应用程序、两个 Azure AD 租户（**T1** 和 **T2**），以及两个权限（**P1** 和 **P2**）。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-136">For example, assume that you have an application, two Azure AD tenants, **T1** and **T2**, and two permissions, **P1** and **P2**.</span></span> <span data-ttu-id="3e4e5-137">以下是授权过程：</span><span class="sxs-lookup"><span data-stu-id="3e4e5-137">The following is the authorization process:</span></span>

- <span data-ttu-id="3e4e5-138">应用程序注册以请求权限 **P1**。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-138">The application registers to require permission **P1**.</span></span>
- <span data-ttu-id="3e4e5-139">当租户 **T1** 中的用户获取此应用程序的 Azure AD 令牌时，该令牌不包含任何权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-139">When users in tenant **T1** get an Azure AD token for this application, the token does not contain any permissions.</span></span>
- <span data-ttu-id="3e4e5-140">租户 **T1** 的 Azure AD 管理员向应用程序显式授予权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-140">The Azure AD admin of tenant **T1** explicitly grants permissions to the application.</span></span> <span data-ttu-id="3e4e5-141">当租户 **T1** 中的用户获取应用程序的 Azure AD 令牌时，它将包含权限 **P1**。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-141">When users in tenant **T1** get an Azure AD token for the application, it will contain permission **P1**.</span></span>
- <span data-ttu-id="3e4e5-142">当租户 **T2** 中的用户获取应用程序的 Azure AD 令牌时，该令牌不包含任何权限，因为租户 **T2** 的管理员尚未向该应用程序授予权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-142">When users in tenant **T2** get an Azure AD token for the application, the token does not contain any permissions - because the admin of tenant **T2** did not yet grant permissions to the application.</span></span> <span data-ttu-id="3e4e5-143">权限必须按照*每个租户*和*每个应用程序*进行授予。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-143">Permission must be granted *per tenant* and *per application*.</span></span>
- <span data-ttu-id="3e4e5-144">应用程序将其注册更改为现在需要权限 **P1** 和 **P2**。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-144">The application has its registration changed to now require permissions **P1** and **P2**.</span></span>
- <span data-ttu-id="3e4e5-145">当租户 **T1** 中的用户获取应用程序的 Azure AD 令牌时，它仅包含权限 **P1**。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-145">When users in tenant **T1** get an Azure AD token for the application, it only contains permission **P1**.</span></span> <span data-ttu-id="3e4e5-146">授予应用程序的权限作为授予内容快照进行记录，它们在应用程序注册（权限）更改后*不会自动更改*。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-146">Permissions granted to an application are recorded as snapshots of what was granted - they *do not change automatically* after the application registration (permission) changes.</span></span>
- <span data-ttu-id="3e4e5-147">租户 **T2** 的管理员对应用程序授予权限 **P1** 和 **P2**。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-147">The admin of tenant **T2** grants permissions **P1** and **P2** to the application.</span></span> <span data-ttu-id="3e4e5-148">当租户 **T2** 中的用户获取应用程序的 Azure AD 令牌时，该令牌将包含权限 **P1** 和 **P2**。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-148">Now, when users in tenant **T2** get an Azure AD token for the application, the token will contain permissions **P1** and **P2**.</span></span>

><span data-ttu-id="3e4e5-149">**注意**：租户 **T1** 中的应用程序和租户 **T2** 中的应用程序的 Azure AD 令牌包含不同权限，因为每个租户管理员已为应用程序授予不同的权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-149">**Note**: The Azure AD tokens for the application in tenant **T1** and the application in tenant **T2** contain different permissions, because each tenant admin has granted different permissions to the application.</span></span>

- <span data-ttu-id="3e4e5-150">如需使租户 **T1** 中的应用程序再次运行，租户 **T1** 的管理员必须向应用程序显式授予权限 **P1** 和 **P2**。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-150">To make the application work again in tenant **T1**, the admin of tenant **T1** must explicitly grant permissions **P1** and **P2** to the application.</span></span>

## <a name="register-an-application-in-the-azure-ad-v20-endpoint"></a><span data-ttu-id="3e4e5-151">在 Azure AD v2.0 终结点中注册应用程序</span><span class="sxs-lookup"><span data-stu-id="3e4e5-151">Register an application in the Azure AD v2.0 endpoint</span></span>

<span data-ttu-id="3e4e5-152">如需将应用程序注册到 Azure AD v2.0 终结点，将需要：</span><span class="sxs-lookup"><span data-stu-id="3e4e5-152">To register an application to the Azure AD v2.0 endpoint, you'll need:</span></span>

- <span data-ttu-id="3e4e5-153">**应用程序名称** - 表示应用程序名称的字符串。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-153">**Application name** - A string used for the application name.</span></span>
- <span data-ttu-id="3e4e5-154">**重定向 URL** - 该 URL 发送来自 Azure AD 的身份验证响应。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-154">**Redirect URL** - The URL where the authentication response from Azure AD is sent.</span></span> <span data-ttu-id="3e4e5-155">请使用测试客户端 web 应用主页以开始。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-155">To start, you can use the test client web app homepage.</span></span>
- <span data-ttu-id="3e4e5-156">**所需的权限** - 应用程序需要的用于调用 Microsoft Graph 的权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-156">**Required Permissions** - The permissions that your application requires to be able to call Microsoft Graph.</span></span>

<span data-ttu-id="3e4e5-157">注册应用程序：</span><span class="sxs-lookup"><span data-stu-id="3e4e5-157">To register your application:</span></span>

1. <span data-ttu-id="3e4e5-158">转到 https://apps.dev.microsoft.com/ 并登录。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-158">Go to https://apps.dev.microsoft.com/ and sign in.</span></span>
    ><span data-ttu-id="3e4e5-159">**注意**：你无需是租户管理员。你将被重定向到“**我的应用程序**”列表。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-159">**Note**: You don't have to be a tenant admin. You will be redirected to the **My applications** list.</span></span>
2. <span data-ttu-id="3e4e5-160">选择“**添加应用**”，并输入“**应用程序名称**”以创建新应用程序。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-160">Choose **Add an app**, and enter an **Application Name** to create a new application.</span></span>
3. <span data-ttu-id="3e4e5-161">在新应用程序注册页面，选择“**添加平台**” > “**Web**”。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-161">On the registration page for the new application, choose **Add Platform** > **Web**.</span></span> <span data-ttu-id="3e4e5-162">在“**重定向 URL**”字段中，输入重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-162">In the **Redirect URL** field, enter the redirect URL.</span></span>
4. <span data-ttu-id="3e4e5-163">在“**Microsoft Graph 权限**”部分的“**委派权限**”下，选择“**添加**”。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-163">In the **Microsoft Graph Permissions** section, under **Delegated Permissions**, choose **Add**.</span></span> <span data-ttu-id="3e4e5-164">在对话框中，选择所需的权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-164">In the dialog box, choose the required permissions.</span></span> <span data-ttu-id="3e4e5-165">如需查看权限列表，请参阅[安全权限](permissions-reference.md#security-permissions)。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-165">For a list of permissions, see [Security permissions](permissions-reference.md#security-permissions).</span></span>

    ><span data-ttu-id="3e4e5-166">Microsoft Graph 安全 API 需要获取查询的 SecurityEvents.Read.All 范围和修补程序/后处理查询的 SecurityEvents.ReadWrite.All 范围。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-166">The Microsoft Graph Security API requires the SecurityEvents.Read.All scope for GET queries, and the SecurityEvents.ReadWrite.All scope for PATCH/POST queries.</span></span>

5. <span data-ttu-id="3e4e5-167">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-167">Choose **Save**.</span></span>

<span data-ttu-id="3e4e5-168">保存以下信息：</span><span class="sxs-lookup"><span data-stu-id="3e4e5-168">Save the following information:</span></span>

- <span data-ttu-id="3e4e5-169">应用程序 ID</span><span class="sxs-lookup"><span data-stu-id="3e4e5-169">Application ID</span></span>
- <span data-ttu-id="3e4e5-170">重定向 URL</span><span class="sxs-lookup"><span data-stu-id="3e4e5-170">Redirect URL</span></span>
- <span data-ttu-id="3e4e5-171">所需权限列表</span><span class="sxs-lookup"><span data-stu-id="3e4e5-171">List of required permissions</span></span>

<span data-ttu-id="3e4e5-172">如需了解更多信息，请参阅[使用 Azure AD v2.0 终结点注册应用](auth-register-app-v2.md)。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-172">For more information, see [Register your app with the Azure AD v2.0 endpoint](auth-register-app-v2.md).</span></span>

## <a name="grant-permissions-to-an-application"></a><span data-ttu-id="3e4e5-173">向应用程序授予权限</span><span class="sxs-lookup"><span data-stu-id="3e4e5-173">Grant permissions to an application</span></span>

<span data-ttu-id="3e4e5-174">应用程序注册仅定义应用程序所需的权限，它并不向应用程序授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-174">Application registration only defines which permission the application requires - it does not grant these permissions to the application.</span></span> <span data-ttu-id="3e4e5-175">Azure AD 租户管理员必须通过调用管理员许可终结点来显示授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-175">An Azure AD tenant administrator must explicitly grant these permissions by making a call to the admin consent endpoint.</span></span> <span data-ttu-id="3e4e5-176">如需了解详细信息，请参阅[使用管理员许可终结点](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-scopes#using-the-admin-consent-endpoint)。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-176">For details, see [Using the admin consent endpoint](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-scopes#using-the-admin-consent-endpoint).</span></span>

<span data-ttu-id="3e4e5-177">如要向应用程序授予权限，将需要：</span><span class="sxs-lookup"><span data-stu-id="3e4e5-177">To grant permissions to an application, you'll need:</span></span>

- <span data-ttu-id="3e4e5-178">**应用程序 ID** - 应用程序注册门户中的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-178">**Application ID** - The application ID from application registration portal.</span></span>
- <span data-ttu-id="3e4e5-179">**重定向 URL** - 在应用程序注册门户中为身份验证响应设置的字符串。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-179">**Redirect URL** - The string you set in the application registration portal for authentication response.</span></span>

<span data-ttu-id="3e4e5-180">如要授予权限，请执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="3e4e5-180">To grant the permissions:</span></span>

- <span data-ttu-id="3e4e5-181">在文本编辑器中创建以下 URL 字符串：</span><span class="sxs-lookup"><span data-stu-id="3e4e5-181">In a text editor, create following URL string:</span></span>

    `https://login.microsoftonline.com/common/adminconsent?client_id=<Application Id>&state=12345&redirect_uri=<Redirect URL>`

- <span data-ttu-id="3e4e5-182">在 web 浏览器中转到此 URL，并以租户管理员身份登录。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-182">In a web browser, go to this URL, and sign in as a tenant administrator.</span></span> <span data-ttu-id="3e4e5-183">对话框将显示应用程序需要的权限列表，如应用程序注册门户中所指定的。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-183">The dialog box shows the list of permission the application requires, as specified in the application registration portal.</span></span> <span data-ttu-id="3e4e5-184">选择“**确定**”，以向应用程序授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-184">Choose **OK** to grant the application these permissions.</span></span>

> <span data-ttu-id="3e4e5-185">**注意：** 此步骤向应用程序授予权限，而不是向用户授权。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-185">**Note:** This step grants permissions to the application - not to users.</span></span> <span data-ttu-id="3e4e5-186">这意味着属于 Azure AD 租户的所有使用此应用程序的用户将被授予权限，甚至包括非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-186">This means that all users belonging to the Azure AD tenant that use this application will be granted these permissions - even non-admin users.</span></span>

## <a name="assign-azure-ad-roles-to-users"></a><span data-ttu-id="3e4e5-187">向用户分配 Azure AD 角色</span><span class="sxs-lookup"><span data-stu-id="3e4e5-187">Assign Azure AD roles to users</span></span>

<span data-ttu-id="3e4e5-188">应用程序被授予权限后，每个可以访问该应用程序的人（即 Azure AD 租户的成员）都将获得已授予的权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-188">After an application is granted permissions, everyone with access to the application (that is, members of the Azure AD tenant) will receive the granted permissions.</span></span> <span data-ttu-id="3e4e5-189">为进一步保护敏感的安全数据，Microsoft Graph 安全 API 还需要 Azure AD**安全读者**角色分配用户。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-189">To further protect sensitive security data, the Microsoft Graph Security API also requires users to be assigned the Azure AD **Security Reader** role.</span></span> <span data-ttu-id="3e4e5-190">如需了解详细信息，请参阅[分配管理员角色](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-assign-admin-roles-azure-portal)和[为用户分配管理员角色](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-users-assign-role-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-190">For details, see [Assigning administrator roles](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-assign-admin-roles-azure-portal) and [Assign a user to adminstrator roles](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-users-assign-role-azure-portal).</span></span>

><span data-ttu-id="3e4e5-191">**注意：** 必须是租户管理员才能执行此步骤。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-191">**Note:** You must be a tenant admin to perform this step.</span></span>

<span data-ttu-id="3e4e5-192">若要为用户分配角色：</span><span class="sxs-lookup"><span data-stu-id="3e4e5-192">To assign roles to users:</span></span>

- <span data-ttu-id="3e4e5-193">登录到 [Azure 门户](https://portal.azure.com) (https://portal.azure.com)。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-193">Sign in to the [azure portal](https://portal.azure.com) (https://portal.azure.com).</span></span>
- <span data-ttu-id="3e4e5-194">在菜单中，选择“**Azure Active Directory**” > “**用户**”。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-194">In the menu, select **Azure Active Directory** > **Users**.</span></span>
- <span data-ttu-id="3e4e5-195">选择用户名称。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-195">Select the name of the user.</span></span>
- <span data-ttu-id="3e4e5-196">选择“**管理**” > “**目录角色**”。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-196">Select **Manage** > **Directory role**.</span></span>
- <span data-ttu-id="3e4e5-197">选择“**有限管理员**”，然后选中“**安全读者**”复选框。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-197">Select **Limited administrator**, and choose the **Security reader** check box.</span></span>
- <span data-ttu-id="3e4e5-198">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-198">Choose **Save**.</span></span>

## <a name="create-an-authentication-code"></a><span data-ttu-id="3e4e5-199">创建身份验证代码</span><span class="sxs-lookup"><span data-stu-id="3e4e5-199">Create an authentication code</span></span>

<span data-ttu-id="3e4e5-200">若要创建身份验证代码，将需要：</span><span class="sxs-lookup"><span data-stu-id="3e4e5-200">To create an authentication code, you'll need:</span></span>

- <span data-ttu-id="3e4e5-201">**应用程序 ID** - 应用程序注册门户中的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-201">**Application ID** - The application ID from application registration portal.</span></span>
- <span data-ttu-id="3e4e5-202">**重定向 URL** - 该 URL 发送来自 Azure AD 的身份验证响应。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-202">**Redirect URL** - The URL where the authentication response from Azure AD is sent.</span></span> <span data-ttu-id="3e4e5-203">请使用 https://localhost 或测试客户端 web 应用主页以开始。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-203">To start, you can use https://localhost or the test client web app homepage.</span></span>
- <span data-ttu-id="3e4e5-204">**应用程序密钥**（可选）- 应用程序的密钥。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-204">**Application Key** (optional) - The key of the application.</span></span> <span data-ttu-id="3e4e5-205">这适用于将使用仅应用程序身份验证代码（即不支持用户委派身份验证）的应用程序的开发。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-205">This applies when you're developing an application that will use application-only authentication code (that is, will not support user delegated authentication).</span></span>

<span data-ttu-id="3e4e5-206">下表列出了可用于创建身份验证代码的资源。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-206">The following table lists resources that you can use to create an authentication code.</span></span>

|<span data-ttu-id="3e4e5-207">**应用程序类型**</span><span class="sxs-lookup"><span data-stu-id="3e4e5-207">**Type of application**</span></span>|<span data-ttu-id="3e4e5-208">**身份验证库**</span><span class="sxs-lookup"><span data-stu-id="3e4e5-208">**Authentication library**</span></span>|
|------------------------|----------------------------|
|[<span data-ttu-id="3e4e5-209">桌面应用 - iOS</span><span class="sxs-lookup"><span data-stu-id="3e4e5-209">Desktop apps - iOS</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/guidedsetups/active-directory-ios)|[<span data-ttu-id="3e4e5-210">MSAL.framework：适用于 iOS 的 Microsoft 身份验证库预览版</span><span class="sxs-lookup"><span data-stu-id="3e4e5-210">MSAL.framework: Microsoft Authentication Library Preview for iOS</span></span>](https://github.com/AzureAD/microsoft-authentication-library-for-objc)|
|[<span data-ttu-id="3e4e5-211">桌面应用 - Android</span><span class="sxs-lookup"><span data-stu-id="3e4e5-211">Desktop apps - Android</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/guidedsetups/active-directory-android)|[<span data-ttu-id="3e4e5-212">Microsoft 身份验证库 (MSAL)</span><span class="sxs-lookup"><span data-stu-id="3e4e5-212">Microsoft Authentication Library (MSAL)</span></span>](https://javadoc.io/doc/com.microsoft.identity.client/msal)|
|[<span data-ttu-id="3e4e5-213">桌面应用 - .Net</span><span class="sxs-lookup"><span data-stu-id="3e4e5-213">Desktop apps - .Net</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/guidedsetups/active-directory-windesktop)|[<span data-ttu-id="3e4e5-214">Microsoft 身份验证库 (MSAL)</span><span class="sxs-lookup"><span data-stu-id="3e4e5-214">Microsoft Authentication Library (MSAL)</span></span>](https://www.nuget.org/packages/Microsoft.Identity.Client)|
|[<span data-ttu-id="3e4e5-215">Web 应用 - JavaScript SPA</span><span class="sxs-lookup"><span data-stu-id="3e4e5-215">Web apps - JavaScript SPA</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/guidedsetups/active-directory-javascriptspa)|[<span data-ttu-id="3e4e5-216">适用于 JavaScript 的 Microsoft 身份验证库预览版</span><span class="sxs-lookup"><span data-stu-id="3e4e5-216">Microsoft Authentication Library for JavaScript Preview</span></span>](https://github.com/AzureAD/microsoft-authentication-library-for-js)|
|[<span data-ttu-id="3e4e5-217">Web 应用 - .NET Web 服务器</span><span class="sxs-lookup"><span data-stu-id="3e4e5-217">Web apps - .NET Web Server</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/guidedsetups/active-directory-aspnetwebapp)|<span data-ttu-id="3e4e5-218">OpenIdConnection、Cookie、SystemWeb</span><span class="sxs-lookup"><span data-stu-id="3e4e5-218">OpenIdConnection, Cookies, SystemWeb</span></span>|
|[<span data-ttu-id="3e4e5-219">Web 应用 - NodeJS Web 应用</span><span class="sxs-lookup"><span data-stu-id="3e4e5-219">Web apps - NodeJS Web App</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-devquickstarts-node-web)||

<span data-ttu-id="3e4e5-220">对于不使用任何现有库的应用程序，请参阅[代表用户获取访问权限](auth-v2-user.md)。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-220">For applications that don't use any of the existing libraries, see [Get access on behalf of a user](auth-v2-user.md).</span></span>

1. <span data-ttu-id="3e4e5-221">从 Azure AD 获取代码。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-221">Get a code from Azure AD.</span></span> <span data-ttu-id="3e4e5-222">调用的查询包含应用程序 ID 参数、重定向 URl 和**所需的权限**。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-222">The query to call contains parameter for Application ID, Redirect URl, and **required permissions**.</span></span>
2. <span data-ttu-id="3e4e5-223">使用代码获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-223">Use the code to get an access token.</span></span>

<span data-ttu-id="3e4e5-224">如果你使用 OpenId Connect 库，请参阅[使用 Azure AD 和 OpenID Connect 进行身份验证](https://docs.microsoft.com/en-us/azure/architecture/multitenant-identity/authenticate)并调用 `app.UseOpenIdConnectAuthentication()`。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-224">If you use OpenId Connect library, see [Authenticate using Azure AD and OpenID Connect](https://docs.microsoft.com/en-us/azure/architecture/multitenant-identity/authenticate) and call `app.UseOpenIdConnectAuthentication()`.</span></span>

><span data-ttu-id="3e4e5-225">**注意：** 如果请求的是用户委派身份验证令牌，库的参数是**请求的作用域**。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-225">**Note:** If you're requesting user delegated authentication tokens, the parameter for the library is **Requested Scopes**.</span></span> <span data-ttu-id="3e4e5-226">请对该参数使用 User.Read，而非注册的应用程序所要求的值。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-226">Use User.Read for this parameter instead of what the registered application requires.</span></span> <span data-ttu-id="3e4e5-227">**请求的作用域**参数不影响包含在返回身份验证令牌中的权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-227">The **Requested Scopes** parameter does NOT affect the permissions contained in the returned authentication tokens.</span></span> <span data-ttu-id="3e4e5-228">这些由租户管理员授予应用程序的权限所确定。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-228">These are determined by the permissions that the tenant admin granted the application.</span></span>

<span data-ttu-id="3e4e5-229">例如，如果使用 .NET MSAL 库，请执行以下调用：</span><span class="sxs-lookup"><span data-stu-id="3e4e5-229">For example, if you're using the .NET MSAL library, call the following:</span></span>

`var accessToken = (await client.AcquireTokenAsync(scopes)).AccessToken;`

><span data-ttu-id="3e4e5-230">**注意：** 此示例应使用最低的许可权限，如 User.Read。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-230">**Note:** This example should use the least privileged permission, such as User.Read.</span></span> <span data-ttu-id="3e4e5-231">但是，返回的访问令牌可包含由租户管理员授予当前用户租户的权限，如 User.Read.All 或 User.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-231">However, the returned access token can contain permissions that were granted by the tenant admin for the current user tenant, such as User.Read.All or User.ReadWrite.All.</span></span>

<span data-ttu-id="3e4e5-232">Azure AD 返回的令牌（字符串）包含身份验证信息和应用程序所需的权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-232">A token (string) is returned by Azure AD that contains your authentication information and the permissions required by the application.</span></span> <span data-ttu-id="3e4e5-233">将此令牌作为持有者令牌分配到 HTTP 标头，如下例所示。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-233">Assign this token to the HTTP header as a bearer token, as shown in the following example.</span></span>

`request.Headers.Authorization = new AuthenticationHeaderValue("bearer", accessToken);`

<span data-ttu-id="3e4e5-234">Microsoft Graph 将验证包含在此令牌中的信息，并授予或拒绝访问权限。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-234">Microsoft Graph will validate the information contained in this token and grant, or reject, access.</span></span>

<span data-ttu-id="3e4e5-235">如要查看包含在返回令牌中的声明，请使用 NuGet 库 System.IdentityModel.Tokens.Jwt。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-235">To view claims contained in the returned token, use NuGet library System.IdentityModel.Tokens.Jwt.</span></span>

`JwtSecurityTokenHandler tokenHandler = new JwtSecurityTokenHandler();`</br>
`var securityToken = tokenHandler.ReadToken(accessToken) as JwtSecurityToken;`

<span data-ttu-id="3e4e5-236">来自 Microsoft Graph 的响应包含一个被称为 client-request-id 的标头，这是一个 GUID。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-236">The response from Microsoft Graph contains a header called client-request-id, which is a GUID.</span></span> <span data-ttu-id="3e4e5-237">如果访问被拒绝，在 [Microsoft 技术社区](https://techcommunity.microsoft.com/t5/Microsoft-Graph-Security-API/ct-p/SecurityGraphAPI)寻求支持时请指明此 GUID，以便帮助调查此身份验证故障的原因。</span><span class="sxs-lookup"><span data-stu-id="3e4e5-237">If access is denied, please specify this GUID when seeking support at [Microsoft Tech Community](https://techcommunity.microsoft.com/t5/Microsoft-Graph-Security-API/ct-p/SecurityGraphAPI), so we can help investigate the cause of this authentication failure.</span></span>
