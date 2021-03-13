---
title: 在没有用户的情况下获取访问权限
description: 一些应用使用他们自己的标识（而不代表用户）调用 Microsoft Graph。 在许多情况下，这些是在服务器上运行的后台服务或守护程序，不存在登录用户。
author: jackson-woods
localization_priority: Priority
ms.prod: applications
ms.custom: graphiamtop20
ms.openlocfilehash: 63b9f184639c3cb7186c65940add3cf9d6b1a47d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761463"
---
# <a name="get-access-without-a-user"></a><span data-ttu-id="c94f3-104">在没有用户的情况下获取访问权限</span><span class="sxs-lookup"><span data-stu-id="c94f3-104">Get access without a user</span></span>

<span data-ttu-id="c94f3-p102">一些应用使用他们自己的标识（而不代表用户）调用 Microsoft Graph。在许多情况下，这些是在的服务器上运行的后台服务或守护程序，不存在登录用户。此类应用的一个示例是电子邮件存档服务，它可以在夜间保持清醒状态并运行。在某些情况下，具有登录用户的应用可能还需要以他们自己的标识调用 Microsoft Graph。例如，应用可能需要使用以下特定功能，该功能要求在组织中具有比登录用户的提升权限更多的权限。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p102">Some apps call Microsoft Graph with their own identity and not on behalf of a user. In many cases, these are background services or daemons that run on a server without the presence of a signed-in user. An example of such an app might be an email archival service that wakes up and runs overnight. In some cases, apps that have a signed-in user present may also need to call Microsoft Graph under their own identity. For example, an app may need to use functionality that requires more elevated privileges in an organization than those carried by the signed-in user.</span></span>  

<span data-ttu-id="c94f3-p103">使用它们自己的标识调用 Microsoft Graph 的应用使用 OAuth 2.0 [客户端凭据授予流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)从 Azure AD 获取访问令牌。本主题介绍了配置服务和使用 OAuth 客户端凭据授予流获取访问令牌的基本步骤。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p103">Apps that call Microsoft Graph with their own identity use the OAuth 2.0 [client credentials grant flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) to get access tokens from Azure AD. This topic describes the basic steps to configure a service and use the OAuth client credentials grant flow to get an access token.</span></span>

## <a name="authentication-and-authorization-steps"></a><span data-ttu-id="c94f3-112">身份验证和授权步骤</span><span class="sxs-lookup"><span data-stu-id="c94f3-112">Authentication and authorization steps</span></span>

<span data-ttu-id="c94f3-113">需要执行下列基本步骤来配置服务并从 Microsoft 标识平台终结点获取你的服务在其自身标识下调用 Microsoft Graph 时所用的令牌：</span><span class="sxs-lookup"><span data-stu-id="c94f3-113">The basic steps required to configure a service and get a token from the Microsoft identity platform endpoint that your service can use to call Microsoft Graph under its own identity are:</span></span>

1. <span data-ttu-id="c94f3-114">注册应用。</span><span class="sxs-lookup"><span data-stu-id="c94f3-114">Register your app.</span></span>
2. <span data-ttu-id="c94f3-115">在应用上配置 Microsoft Graph 的权限。</span><span class="sxs-lookup"><span data-stu-id="c94f3-115">Configure permissions for Microsoft Graph on your app.</span></span>
3. <span data-ttu-id="c94f3-116">获取管理员同意。</span><span class="sxs-lookup"><span data-stu-id="c94f3-116">Get administrator consent.</span></span>
4. <span data-ttu-id="c94f3-117">获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="c94f3-117">Get an access token.</span></span>
5. <span data-ttu-id="c94f3-118">使用访问令牌调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="c94f3-118">Use the access token to call Microsoft Graph.</span></span>

## <a name="1-register-your-app"></a><span data-ttu-id="c94f3-119">1.注册你的应用程序</span><span class="sxs-lookup"><span data-stu-id="c94f3-119">1. Register your app</span></span>

<span data-ttu-id="c94f3-p104">要向 Microsoft 标识平台终结点进行身份验证，必须先在 [Azure 应用注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)注册你的应用。你可使用 Microsoft 帐户或工作/学校帐户来注册应用。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p104">To authenticate with the Microsoft identity platform endpoint, you must first register your app at the [Azure app registration portal](https://go.microsoft.com/fwlink/?linkid=2083908). You can use either a Microsoft account or a work or school account to register your app.</span></span>

<span data-ttu-id="c94f3-122">对于将以自己的标识调用 Microsoft Graph 的服务，用户需要将应用注册到 Web 平台并复制以下值：</span><span class="sxs-lookup"><span data-stu-id="c94f3-122">For a service that will call Microsoft Graph under its own identity, you need to register your app for the Web platform and copy the following values:</span></span>

- <span data-ttu-id="c94f3-123">Azure 应用注册门户分配的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="c94f3-123">The Application ID assigned by the Azure app registration portal.</span></span>
- <span data-ttu-id="c94f3-124">客户端（应用程序）密码，它是一个密码或是一个公钥/私钥对（证书）。</span><span class="sxs-lookup"><span data-stu-id="c94f3-124">A Client (application) Secret, either a password or a public/private key pair (certificate).</span></span>
- <span data-ttu-id="c94f3-125">服务用于接收令牌响应的重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="c94f3-125">A Redirect URL for your service to receive token responses.</span></span>
- <span data-ttu-id="c94f3-126">服务用于接收管理员同意答复的重定向 URL（在你的应用实现功能来请求管理员同意的情况下）。</span><span class="sxs-lookup"><span data-stu-id="c94f3-126">A Redirect URL for your service to receive admin consent responses if your app implements functionality to request administrator consent.</span></span>  

<span data-ttu-id="c94f3-127">要分步了解如何通过 Azure 应用注册门户配置应用，请参阅[注册应用](./auth-register-app-v2.md)。</span><span class="sxs-lookup"><span data-stu-id="c94f3-127">For steps on how to configure an app using the Azure app registration portal, see [Register your app](./auth-register-app-v2.md).</span></span>

<span data-ttu-id="c94f3-128">借助 OAuth 2.0 客户端凭据授予流，你的应用可通过 Azure AD 分配的应用程序 ID 以及依靠门户创建的应用程序密码在 Microsoft 标识平台 `/token` 终结点处直接进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="c94f3-128">With the OAuth 2.0 client credentials grant flow, your app authenticates directly at the Microsoft identity platform `/token` endpoint using the Application ID assigned by Azure AD and the Application Secret that you create using the portal.</span></span>

## <a name="2-configure-permissions-for-microsoft-graph"></a><span data-ttu-id="c94f3-129">2.配置 Microsoft Graph 的权限</span><span class="sxs-lookup"><span data-stu-id="c94f3-129">2. Configure permissions for Microsoft Graph</span></span>

<span data-ttu-id="c94f3-p105">对于以它们自己的标识调用 Microsoft Graph 的应用，Microsoft Graph 显示应用程序权限。（Microsoft Graph 还显示代表用户调用 Microsoft Graph 的应用的委派权限。）注册应用时，需要预配置应用所需的应用程序权限。应用程序权限始终需要管理员的同意。当你的应用安装在他们的组织中时，管理员可以使用 [Azure 门户](https://portal.azure.com)同意这些权限，你也可以提供应用注册体验，让管理员同意你配置的权限。Azure AD 记录管理员同意后，你的应用无需再次请求同意即可请求令牌。有关可通过 Microsoft Graph 使用的权限的详细信息，请参阅[权限参考](./permissions-reference.md)</span><span class="sxs-lookup"><span data-stu-id="c94f3-p105">For apps that call Microsoft Graph under their own identity, Microsoft Graph exposes application permissions (Microsoft Graph can also expose delegated permissions for apps that call Microsoft Graph on behalf of a user). You pre-configure the application permissions your app needs when you register your app. Application permissions always require administrator consent. An administrator can either consent to these permissions using the [Azure portal](https://portal.azure.com) when your app is installed in their organization, or you can provide a sign-up experience in your app through which administrators can consent to the permissions you configured. Once administrator consent is recorded by Azure AD, your app can request tokens without having to request consent again. For more detailed information about the permissions available with Microsoft Graph, see the [Permissions reference](./permissions-reference.md)</span></span>

<span data-ttu-id="c94f3-136">若要在 [Azure 应用注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)为应用配置应用程序权限：在应用程序的 **API 权限** 页面中，选择“**添加权限**”，选择“**Microsoft Graph**”，然后在“**应用程序权限**”下选择你的应用所需的权限。</span><span class="sxs-lookup"><span data-stu-id="c94f3-136">To configure application permissions for your app in the [Azure app registrations portal](https://go.microsoft.com/fwlink/?linkid=2083908): under an application's **API permissions** page, choose **Add a permission**, select **Microsoft Graph**, and then choose the permissions your app requires under **Application permissions**.</span></span>

<span data-ttu-id="c94f3-137">下面的屏幕快照显示了 Microsoft Graph 应用程序权限的“**选择权限**”对话框。</span><span class="sxs-lookup"><span data-stu-id="c94f3-137">The following screenshot shows the **Select Permissions** dialog box for Microsoft Graph application permissions.</span></span>

![Microsoft Graph 应用程序权限的“选择权限”对话框。](./images/auth-v2/v2-application-permissions.png)

> <span data-ttu-id="c94f3-p106">**注意**：建议配置应用需要的最小特权权限集。这为管理员提供的体验要比不得不同意一个很长的权限列表的体验舒适得多。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p106">**Note**: We recommend that you configure the least privileged set of permissions required by your app. This provides a much more comfortable experience for administrators than having to consent to a long list of permissions.</span></span>

## <a name="3-get-administrator-consent"></a><span data-ttu-id="c94f3-141">3.获取管理员同意</span><span class="sxs-lookup"><span data-stu-id="c94f3-141">3. Get administrator consent</span></span>

<span data-ttu-id="c94f3-142">你可让管理员在 [Azure 门户](https://portal.azure.com)授予你的应用所需的权限；但通常情况下，更好的方法是通过 Microsoft 标识平台 `/adminconsent` 终结点提供管理员注册体验。</span><span class="sxs-lookup"><span data-stu-id="c94f3-142">You can rely on an administrator to grant the permissions your app needs at the [Azure portal](https://portal.azure.com); however, often, a better option is to provide a sign-up experience for administrators by using the Microsoft identity platform `/adminconsent` endpoint.</span></span> 

> <span data-ttu-id="c94f3-143">**重要说明**：任何时候更改配置权限都必须重复管理员同意过程。</span><span class="sxs-lookup"><span data-stu-id="c94f3-143">**Important**: Any time you make a change to the configured permissions, you must also repeat the Admin Consent process.</span></span> <span data-ttu-id="c94f3-144">租户管理员重新应用同意之后，才会反映应用注册门户中所做的更改。</span><span class="sxs-lookup"><span data-stu-id="c94f3-144">Changes made in the app registration portal will not be reflected until consent has been reapplied by the tenant's administrator.</span></span>

### <a name="request"></a><span data-ttu-id="c94f3-145">请求</span><span class="sxs-lookup"><span data-stu-id="c94f3-145">Request</span></span>

```
// Line breaks are for legibility only.

GET https://login.microsoftonline.com/{tenant}/adminconsent
?client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&state=12345
&redirect_uri=https://localhost/myapp/permissions
```

| <span data-ttu-id="c94f3-146">参数</span><span class="sxs-lookup"><span data-stu-id="c94f3-146">Parameter</span></span>     | <span data-ttu-id="c94f3-147">条件</span><span class="sxs-lookup"><span data-stu-id="c94f3-147">Condition</span></span>   | <span data-ttu-id="c94f3-148">说明</span><span class="sxs-lookup"><span data-stu-id="c94f3-148">Description</span></span> 
|:--------------|:------------|:------------
| <span data-ttu-id="c94f3-149">租户</span><span class="sxs-lookup"><span data-stu-id="c94f3-149">tenant</span></span>        | <span data-ttu-id="c94f3-150">必需</span><span class="sxs-lookup"><span data-stu-id="c94f3-150">Required</span></span>    | <span data-ttu-id="c94f3-p108">需要从中请求权限的目录租户。它可以 GUID 或友好名称格式显示。如果你不了解用户授予哪个租户，并想让用户使用任意租户登录，请使用 `common`。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p108">The directory tenant that you want to request permission from. This can be in GUID or friendly name format. If you don't know which tenant the user belongs to and you want to let them sign in with any tenant, use `common`.</span></span>
| <span data-ttu-id="c94f3-154">client_id</span><span class="sxs-lookup"><span data-stu-id="c94f3-154">client_id</span></span>     | <span data-ttu-id="c94f3-155">必需</span><span class="sxs-lookup"><span data-stu-id="c94f3-155">Required</span></span>    | <span data-ttu-id="c94f3-156">[Azure 应用注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)分配给你的应用的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="c94f3-156">The Application ID that the [Azure app registration portal](https://go.microsoft.com/fwlink/?linkid=2083908) assigned to your app.</span></span>
| <span data-ttu-id="c94f3-157">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="c94f3-157">redirect_uri</span></span>  | <span data-ttu-id="c94f3-158">必需</span><span class="sxs-lookup"><span data-stu-id="c94f3-158">Required</span></span>    | <span data-ttu-id="c94f3-p109">要向其发送响应供应用处理的重定向 URI。它必须完全匹配在门户中注册的重定向 URI 之一，但它必须采用 URL 编码，且可以拥有其他路径段。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p109">The redirect URI where you want the response to be sent for your app to handle. It must exactly match one of the redirect URIs that you registered in the portal, except that it must be URL encoded, and it can have additional path segments.</span></span>
| <span data-ttu-id="c94f3-161">state</span><span class="sxs-lookup"><span data-stu-id="c94f3-161">state</span></span>         | <span data-ttu-id="c94f3-162">建议</span><span class="sxs-lookup"><span data-stu-id="c94f3-162">Recommended</span></span> | <span data-ttu-id="c94f3-p110">请求中包含的值，也会在令牌响应中返回。它可以是你希望的任何内容的字符串。此状态用于在发生身份验证请求前，对应用中的用户状态信息进行编码（例如它们所在的页面或视图上）。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p110">A value that is included in the request that also is returned in the token response. It can be a string of any content that you want. The state is used to encode information about the user's state in the app before the authentication request occurred, such as the page or view they were on.</span></span>

### <a name="administrator-consent-experience"></a><span data-ttu-id="c94f3-166">管理员同意体验</span><span class="sxs-lookup"><span data-stu-id="c94f3-166">Administrator consent experience</span></span>

<span data-ttu-id="c94f3-p111">对于 `/adminconsent` 终结点的请求，Azure AD 强制规定，仅租户管理员可以登录来完成请求。系统可能会提示管理员批准你在应用注册门户中为应用请求获取的所有应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p111">With requests to the `/adminconsent` endpoint, Azure AD enforces that only a tenant administrator can sign in to complete the request. The administrator will be asked to approve all the application permissions that you have requested for your app in the app registration portal.</span></span>

<span data-ttu-id="c94f3-169">下面的示例展示了 Azure AD 向管理员显示的同意对话框：</span><span class="sxs-lookup"><span data-stu-id="c94f3-169">The following is an example of the consent dialog that Azure AD presents to the administrator:</span></span>

![管理员同意对话框。](./images/admin-consent.png)

### <a name="response"></a><span data-ttu-id="c94f3-171">响应</span><span class="sxs-lookup"><span data-stu-id="c94f3-171">Response</span></span>

<span data-ttu-id="c94f3-172">如果管理员批准应用程序的权限，则成功响应如下所示：</span><span class="sxs-lookup"><span data-stu-id="c94f3-172">If the administrator approves the permissions for your application, the successful response looks like this:</span></span>

```
// Line breaks are for legibility only.

GET https://localhost/myapp/permissions
?tenant=a8990e1f-ff32-408a-9f8e-78d3b9139b95&state=12345
&admin_consent=True
```

| <span data-ttu-id="c94f3-173">参数</span><span class="sxs-lookup"><span data-stu-id="c94f3-173">Parameter</span></span>     | <span data-ttu-id="c94f3-174">说明</span><span class="sxs-lookup"><span data-stu-id="c94f3-174">Description</span></span>
|:--------------|:------------
| <span data-ttu-id="c94f3-175">租户</span><span class="sxs-lookup"><span data-stu-id="c94f3-175">tenant</span></span>        | <span data-ttu-id="c94f3-176">以 GUID 格式向应用程序授予其请求的权限的目录租户。</span><span class="sxs-lookup"><span data-stu-id="c94f3-176">The directory tenant that granted your application the permissions that it requested, in GUID format.</span></span>
| <span data-ttu-id="c94f3-177">state</span><span class="sxs-lookup"><span data-stu-id="c94f3-177">state</span></span>         | <span data-ttu-id="c94f3-p112">请求中包含的值，也会在令牌响应中返回。它可以是你希望的任何内容的字符串。此状态用于在发生身份验证请求前，对应用中的用户状态信息进行编码（例如它们所在的页面或视图上）。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p112">A value that is included in the request that also is returned in the token response. It can be a string of any content that you want. The state is used to encode information about the user's state in the app before the authentication request occurred, such as the page or view they were on.</span></span>
| <span data-ttu-id="c94f3-181">admin_consent</span><span class="sxs-lookup"><span data-stu-id="c94f3-181">admin_consent</span></span> | <span data-ttu-id="c94f3-182">设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="c94f3-182">Set to **true**.</span></span>


> <span data-ttu-id="c94f3-p113">**试一试**：可以通过将下面的请求粘贴到浏览器中自行尝试。如果以 Azure AD 租户的全局管理员身份登录，你将看到应用的管理员同意对话框。（这与上文的同意对话框屏幕截图中显示的应用不同。）</span><span class="sxs-lookup"><span data-stu-id="c94f3-p113">**Try**: You can try this for yourself by pasting the following request in a browser. If you sign in as a Global administrator for an Azure AD tenant, you will be presented with the administrator consent dialog box for the app. (This will be a different app than that in the consent dialog box screenshot shown earlier.)</span></span>
> 
> https://login.microsoftonline.com/common/adminconsent?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&state=12345&redirect_uri=https://localhost/myapp/permissions 

## <a name="4-get-an-access-token"></a><span data-ttu-id="c94f3-186">4. 获取访问令牌</span><span class="sxs-lookup"><span data-stu-id="c94f3-186">4. Get an access token</span></span>

<span data-ttu-id="c94f3-187">在 OAuth 2.0 客户端凭据授予流中，可使用在注册应用时保存的应用程序 ID 和应用程序密码值直接从 Microsoft 标识平台 `/token` 终结点请求访问令牌。</span><span class="sxs-lookup"><span data-stu-id="c94f3-187">In the OAuth 2.0 client credentials grant flow, you use the Application ID and Application Secret values that you saved when you registered your app to request an access token directly from the Microsoft identity platform `/token` endpoint.</span></span>

<span data-ttu-id="c94f3-p114">你可以通过传递 `https://graph.microsoft.com/.default` 并将其作为令牌请求中 `scope` 参数的值来指定预配置的权限。请参阅下面的令牌请求中的 `scope` 参数说明获取详情。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p114">You specify the pre-configured permissions by passing `https://graph.microsoft.com/.default` as the value for the `scope` parameter in the token request. See the `scope` parameter description in the token request below for details.</span></span>

### <a name="token-request"></a><span data-ttu-id="c94f3-190">令牌请求</span><span class="sxs-lookup"><span data-stu-id="c94f3-190">Token request</span></span>

<span data-ttu-id="c94f3-191">可将 POST 请求发送到 `/token` 标识平台终结点来获取访问令牌：</span><span class="sxs-lookup"><span data-stu-id="c94f3-191">You send a POST request to the `/token` identity platform endpoint to acquire an access token:</span></span>

```
// Line breaks are for legibility only.

POST https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token HTTP/1.1
Host: login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=535fb089-9ff3-47b6-9bfb-4f1264799865
&scope=https%3A%2F%2Fgraph.microsoft.com%2F.default
&client_secret=qWgdYAmab0YSkuL1qKv5bPX
&grant_type=client_credentials
```

| <span data-ttu-id="c94f3-192">参数</span><span class="sxs-lookup"><span data-stu-id="c94f3-192">Parameter</span></span>     | <span data-ttu-id="c94f3-193">条件</span><span class="sxs-lookup"><span data-stu-id="c94f3-193">Condition</span></span> | <span data-ttu-id="c94f3-194">说明</span><span class="sxs-lookup"><span data-stu-id="c94f3-194">Description</span></span> 
|:--------------|:----------|:------------
| <span data-ttu-id="c94f3-195">租户</span><span class="sxs-lookup"><span data-stu-id="c94f3-195">tenant</span></span>        | <span data-ttu-id="c94f3-196">必需</span><span class="sxs-lookup"><span data-stu-id="c94f3-196">Required</span></span>  | <span data-ttu-id="c94f3-p115">需要从中请求权限的目录租户。它可以 GUID 或友好名称格式显示。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p115">The directory tenant that you want to request permission from. This can be in GUID or friendly name format.</span></span>
| <span data-ttu-id="c94f3-199">client_id</span><span class="sxs-lookup"><span data-stu-id="c94f3-199">client_id</span></span>     | <span data-ttu-id="c94f3-200">必需</span><span class="sxs-lookup"><span data-stu-id="c94f3-200">Required</span></span>  | <span data-ttu-id="c94f3-201">注册应用时由 [Azure 应用注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)分配的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="c94f3-201">The Application ID that the [Azure app registration portal](https://go.microsoft.com/fwlink/?linkid=2083908) assigned when you registered your app.</span></span>
| <span data-ttu-id="c94f3-202">范围</span><span class="sxs-lookup"><span data-stu-id="c94f3-202">scope</span></span>         | <span data-ttu-id="c94f3-203">必需</span><span class="sxs-lookup"><span data-stu-id="c94f3-203">Required</span></span>  | <span data-ttu-id="c94f3-204">为此请求中的 `scope` 参数传递的值应为所需资源的资源标识符（应用程序 ID URI），带有 `.default` 后缀。</span><span class="sxs-lookup"><span data-stu-id="c94f3-204">The value passed for the `scope` parameter in this request should be the resource identifier (Application ID URI) of the resource you want, affixed with the `.default` suffix.</span></span> <span data-ttu-id="c94f3-205">对于 Microsoft Graph，值为 `https://graph.microsoft.com/.default`。</span><span class="sxs-lookup"><span data-stu-id="c94f3-205">For Microsoft Graph, the value is `https://graph.microsoft.com/.default`.</span></span> <span data-ttu-id="c94f3-206">通过该值，Microsoft 标识平台终结点可知晓在你为应用分配的所有应用程序权限中，它应对与你要使用的资源关联的权限颁发令牌。</span><span class="sxs-lookup"><span data-stu-id="c94f3-206">This value informs the Microsoft identity platform endpoint that of all the application permissions you have configured for your app, it should issue a token for the ones associated with the resource you want to use.</span></span>
| <span data-ttu-id="c94f3-207">client_secret</span><span class="sxs-lookup"><span data-stu-id="c94f3-207">client_secret</span></span> | <span data-ttu-id="c94f3-208">必需</span><span class="sxs-lookup"><span data-stu-id="c94f3-208">Required</span></span>  | <span data-ttu-id="c94f3-209">你在应用注册门户中为应用生成的应用程序密码。</span><span class="sxs-lookup"><span data-stu-id="c94f3-209">The Application Secret that you generated for your app in the app registration portal.</span></span>
| <span data-ttu-id="c94f3-210">grant_type</span><span class="sxs-lookup"><span data-stu-id="c94f3-210">grant_type</span></span>    | <span data-ttu-id="c94f3-211">必需</span><span class="sxs-lookup"><span data-stu-id="c94f3-211">Required</span></span>  | <span data-ttu-id="c94f3-212">必须是 `client_credentials`。</span><span class="sxs-lookup"><span data-stu-id="c94f3-212">Must be `client_credentials`.</span></span>

#### <a name="token-response"></a><span data-ttu-id="c94f3-213">令牌响应</span><span class="sxs-lookup"><span data-stu-id="c94f3-213">Token response</span></span>

<span data-ttu-id="c94f3-214">成功的响应如下所示：</span><span class="sxs-lookup"><span data-stu-id="c94f3-214">A successful response looks like this:</span></span>

```json
{
  "token_type": "Bearer",
  "expires_in": 3599,
  "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik1uQ19WWmNBVGZNNXBP..."
}
```

| <span data-ttu-id="c94f3-215">参数</span><span class="sxs-lookup"><span data-stu-id="c94f3-215">Parameter</span></span>     | <span data-ttu-id="c94f3-216">说明</span><span class="sxs-lookup"><span data-stu-id="c94f3-216">Description</span></span>
|:--------------|:------------
| <span data-ttu-id="c94f3-217">access_token</span><span class="sxs-lookup"><span data-stu-id="c94f3-217">access_token</span></span>  | <span data-ttu-id="c94f3-p117">请求的访问令牌。应用可使用此令牌调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p117">The requested access token. Your app can use this token in calls to Microsoft Graph.</span></span>
| <span data-ttu-id="c94f3-220">token_type</span><span class="sxs-lookup"><span data-stu-id="c94f3-220">token_type</span></span>    | <span data-ttu-id="c94f3-p118">表示令牌类型值。Azure AD 唯一支持的类型是 `bearer`</span><span class="sxs-lookup"><span data-stu-id="c94f3-p118">Indicates the token type value. The only type that Azure AD supports is `bearer`.</span></span>
| <span data-ttu-id="c94f3-223">expires_in</span><span class="sxs-lookup"><span data-stu-id="c94f3-223">expires_in</span></span>    | <span data-ttu-id="c94f3-224">访问令牌的有效期是多久（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="c94f3-224">How long the access token is valid (in seconds).</span></span>

## <a name="5-use-the-access-token-to-call-microsoft-graph"></a><span data-ttu-id="c94f3-225">5.使用访问令牌调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c94f3-225">5. Use the access token to call Microsoft Graph</span></span>

<span data-ttu-id="c94f3-p119">拥有访问令牌之后，可以通过将其包含在请求的 `Authorization` 标头中，用其调用 Microsoft Graph。以下请求可以获取特定用户的个人资料。你的应用必须拥有 _User.Read.All_ 权限才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p119">After you have an access token, you can use it to call Microsoft Graph by including it in the `Authorization` header of a request. The following request gets the profile of a specific user. Your app must have the _User.Read.All_ permission to call this API.</span></span>

```
GET https://graph.microsoft.com/v1.0/users/12345678-73a6-4952-a53a-e9916737ff7f
Authorization: Bearer eyJ0eXAiO ... 0X2tnSQLEANnSPHY0gKcgw
Host: graph.microsoft.com
```
<span data-ttu-id="c94f3-229">成功的响应将与此类似（一些响应标头已被删除）：</span><span class="sxs-lookup"><span data-stu-id="c94f3-229">A successful response will look similar to this (some response headers have been removed):</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
request-id: f45d08c0-6901-473a-90f5-7867287de97f
client-request-id: f45d08c0-6901-473a-90f5-7867287de97f
OData-Version: 4.0
Duration: 309.0273
Date: Wed, 26 Apr 2017 19:53:49 GMT
Content-Length: 407
```

```json
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id":"12345678-73a6-4952-a53a-e9916737ff7f",
    "businessPhones":[
        "+1 555555555"
    ],
    "displayName":"Chris Green",
    "givenName":"Chris",
    "jobTitle":"Software Engineer",
    "mail":null,
    "mobilePhone":"+1 5555555555",
    "officeLocation":"Seattle Office",
    "preferredLanguage":null,
    "surname":"Green",
    "userPrincipalName":"ChrisG@contoso.onmicrosoft.com"
}
```

## <a name="supported-app-scenarios-and-resources"></a><span data-ttu-id="c94f3-230">受支持的应用场景和资源</span><span class="sxs-lookup"><span data-stu-id="c94f3-230">Supported app scenarios and resources</span></span>

<span data-ttu-id="c94f3-231">以它们自己的标识调用 Microsoft Graph 的应用可分为两个类别：</span><span class="sxs-lookup"><span data-stu-id="c94f3-231">Apps that call Microsoft Graph under their own identity fall into one of two categories:</span></span>

- <span data-ttu-id="c94f3-232">在服务器上运行的没有登录用户的[后台服务（守护程序）](/azure/active-directory/develop/scenario-daemon-overview)。</span><span class="sxs-lookup"><span data-stu-id="c94f3-232">[Background services (daemons)](/azure/active-directory/develop/scenario-daemon-overview) that run on a server without a signed-in user.</span></span>
- <span data-ttu-id="c94f3-233">具有登录用户但仍以它们自己的标识调用 Microsoft Graph 的应用；例如，使用需要具有比登录用户所拥有的提升权限更多权限的功能。</span><span class="sxs-lookup"><span data-stu-id="c94f3-233">Apps that have a signed-in user but also call Microsoft Graph with their own identity; for example, to use functionality that requires more elevated privileges than those of the user.</span></span>

<span data-ttu-id="c94f3-234">通过自有标识调用 Microsoft Graph 的应用使用 OAuth 2.0 客户端凭据授予流向 Azure AD 进行身份验证并获取令牌。</span><span class="sxs-lookup"><span data-stu-id="c94f3-234">Apps that call Microsoft Graph with their own identity use the OAuth 2.0 client credentials grant to authenticate with Azure AD and get a token.</span></span> <span data-ttu-id="c94f3-235">对于 Microsoft 标识平台终结点，可在下述资源中进一步查看此方案：</span><span class="sxs-lookup"><span data-stu-id="c94f3-235">For the Microsoft identity platform endpoint, you can explore this scenario further with the following resources:</span></span>

- <span data-ttu-id="c94f3-236">有关还包含错误响应的客户端凭据授予流的更完整的处理，请参阅 [Azure Active Directory v2.0 和 OAuth 2.0 客户端凭据流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)。</span><span class="sxs-lookup"><span data-stu-id="c94f3-236">For a more complete treatment of the client credentials grant flow that also includes error responses, see [Azure Active Directory v2.0 and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>
- <span data-ttu-id="c94f3-237">有关从服务中调用 Microsoft Graph 的示例，请参阅 GitHub 上的 [v2.0 守护程序示例](https://github.com/Azure-Samples/active-directory-dotnet-daemon-v2)。</span><span class="sxs-lookup"><span data-stu-id="c94f3-237">For a sample that calls Microsoft Graph from a service, see the [v2.0 daemon sample](https://github.com/Azure-Samples/active-directory-dotnet-daemon-v2) on GitHub.</span></span>
- <span data-ttu-id="c94f3-238">要详细了解所推荐的 Microsoft 和第三方身份验证库，请参阅 [ 标识平台身份验证库](/azure/active-directory/develop/reference-v2-libraries)。</span><span class="sxs-lookup"><span data-stu-id="c94f3-238">For more information about recommended Microsoft and third-party authentication libraries, see [Microsoft identity platform authentication libraries](/azure/active-directory/develop/reference-v2-libraries).</span></span>

## <a name="endpoint-considerations"></a><span data-ttu-id="c94f3-239">终结点注意事项</span><span class="sxs-lookup"><span data-stu-id="c94f3-239">Endpoint considerations</span></span>

<span data-ttu-id="c94f3-240">Microsoft 继续支持 Azure AD 终结点。</span><span class="sxs-lookup"><span data-stu-id="c94f3-240">Microsoft continues to support the Azure AD endpoint.</span></span> <span data-ttu-id="c94f3-241">在使用 Microsoft 标识平台终结点和使用 Azure AD 终结点之间存在[诸多区别](/azure/active-directory/develop/azure-ad-endpoint-comparison)。</span><span class="sxs-lookup"><span data-stu-id="c94f3-241">There are [several differences](/azure/active-directory/develop/azure-ad-endpoint-comparison) between using the Microsoft identity platform endpoint and the Azure AD endpoint.</span></span> <span data-ttu-id="c94f3-242">使用 Azure AD 终结点时：</span><span class="sxs-lookup"><span data-stu-id="c94f3-242">When using the Azure AD endpoint:</span></span>

- <span data-ttu-id="c94f3-243">如果你的应用是多租户的，则必须在 [Azure 门户](https://portal.azure.com)中将其明确配置为“多租户”。</span><span class="sxs-lookup"><span data-stu-id="c94f3-243">If your app is a multi-tenant app, you must explicitly configure it to be multi-tenant in the [Azure portal](https://portal.azure.com).</span></span>
- <span data-ttu-id="c94f3-244">没有管理员同意终结点 (`/adminconsent`)。</span><span class="sxs-lookup"><span data-stu-id="c94f3-244">There is no admin consent endpoint (`/adminconsent`).</span></span> <span data-ttu-id="c94f3-245">你的应用转而可在运行时期间请求管理员同意，方式是向授权请求添加 `prompt=admin_consent` 参数。</span><span class="sxs-lookup"><span data-stu-id="c94f3-245">Instead, your app can request administrator consent during runtime by adding the `prompt=admin_consent` parameter to an authorization request.</span></span> <span data-ttu-id="c94f3-246">有关详细信息，请参阅 [将应用程序与 Azure Active Directory 相集成](/azure/active-directory/develop/active-directory-integrating-applications)中的 **在运行时引发 Azure AD 同意框架**。</span><span class="sxs-lookup"><span data-stu-id="c94f3-246">For more information, see **Triggering the Azure AD consent framework at runtime** in [Integrating applications with Azure Active Directory](/azure/active-directory/develop/active-directory-integrating-applications).</span></span>
- <span data-ttu-id="c94f3-p123">授权和令牌请求中的参数不相同。例如，Azure AD 终结点请求中没有 `scope` 参数；但是，`resource` 参数可用于指定为其请求的授权（用于管理员同意）或令牌的资源 (`resource=https://graph.microsoft.com`) 的 URI。</span><span class="sxs-lookup"><span data-stu-id="c94f3-p123">The parameters in authorization and token requests are different. For example, there is no `scope` parameter in Azure AD endpoint requests; instead, the `resource` parameter is used to specify the URI of the resource (`resource=https://graph.microsoft.com`) that authorization (for administrator consent) or a token is being requested for.</span></span>

<span data-ttu-id="c94f3-249">可查看下述资源进一步了解此方案：</span><span class="sxs-lookup"><span data-stu-id="c94f3-249">You can explore this scenario further with the following resources:</span></span>

- <span data-ttu-id="c94f3-250">要了解如何将 Microsoft 标识平台与不同类型的应用结合使用，请参阅 [Microsoft 标识平台文档](/azure/active-directory/develop/active-directory-developers-guide)中的 **开始使用** 链接。</span><span class="sxs-lookup"><span data-stu-id="c94f3-250">For information about using the Microsoft identity platform with different kinds of apps, see the **Get Started** links in the [Microsoft identity platform documentation](/azure/active-directory/develop/active-directory-developers-guide).</span></span> <span data-ttu-id="c94f3-251">该指南包含众多链接，可通过它们查看 Microsoft 标识平台支持的不同类型的应用的概述主题、快速入门、教程、代码示例和协议文档。</span><span class="sxs-lookup"><span data-stu-id="c94f3-251">The guide contains links to overview topics, quickstarts, tutorials, code samples, and protocol documentation for different kinds of apps supported by the Microsoft identity platform.</span></span>
- <span data-ttu-id="c94f3-252">要了解可与 Microsoft 标识平台终结点结合使用的 Microsoft 身份验证库 (MSAL) 和服务器中间件，请参阅 [Microsoft 身份验证库](/azure/active-directory/develop/active-directory-authentication-libraries)。</span><span class="sxs-lookup"><span data-stu-id="c94f3-252">For information about the Microsoft Authentication Library (MSAL) and server middleware available for use with the Microsoft identity platform endpoint, see [Microsoft Authentication Libraries](/azure/active-directory/develop/active-directory-authentication-libraries).</span></span>