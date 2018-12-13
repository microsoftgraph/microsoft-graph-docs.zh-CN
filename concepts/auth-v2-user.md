---
title: 代表用户访问
description: '若要代表用户使用 Microsoft Graph 读取和写入资源，应用必须从 Azure AD 获取访问令牌，并将令牌附加到其发往 Microsoft Graph 的请求。你将用于获取访问令牌的确切的身份验证流会依赖于你正在开发的应用类型以及你是否要使用 OpenID Connect 让用户登录到应用中。本机和移动应用还有某些 Web 应用使用的常见流程就是 OAuth 2.0 授权代码授予流程。在本主题中，我们将介绍一个使用此流程的示例。 '
ms.openlocfilehash: 136bb917595885f188c2ad6958dc107021b58d10
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091873"
---
# <a name="get-access-on-behalf-of-a-user"></a><span data-ttu-id="065ab-106">代表用户访问</span><span class="sxs-lookup"><span data-stu-id="065ab-106">Get access on behalf of a user</span></span>
<span data-ttu-id="065ab-p102">若要代表用户使用 Microsoft Graph 读取和写入资源，应用必须从 Azure AD 获取访问令牌，并将令牌附加到其发往 Microsoft Graph 的请求。你将用于获取访问令牌的确切的身份验证流会依赖于你正在开发的应用类型以及你是否要使用 OpenID Connect 让用户登录到应用中。本机和移动应用还有某些 Web 应用使用的常见流程就是 OAuth 2.0 授权代码授予流程。在本主题中，我们将介绍一个使用此流程的示例。</span><span class="sxs-lookup"><span data-stu-id="065ab-p102">To use Microsoft Graph to read and write resources on behalf of a user, your app must get an access token from Azure AD and attach the token to requests that it sends to Microsoft Graph. The exact authentication flow that you will use to get access tokens will depend on the kind of app you are developing and whether you want to use OpenID Connect to sign the user in to your app. One common flow used by native and mobile apps and also by some Web apps is the OAuth 2.0 authorization code grant flow. In this topic, we will walk through an example using this flow.</span></span> 

## <a name="authentication-and-authorization-steps"></a><span data-ttu-id="065ab-111">身份验证和授权步骤</span><span class="sxs-lookup"><span data-stu-id="065ab-111">Authentication and Authorization steps</span></span>

<span data-ttu-id="065ab-112">使用 OAuth 2.0 授权代码授予流程从 Azure AD v2.0 终结点获取访问令牌的基本步骤如下：</span><span class="sxs-lookup"><span data-stu-id="065ab-112">The basic steps required to use the OAuth 2.0 authorization code grant flow to get an access token from the Azure AD v2.0 endpoint are:</span></span>

1. <span data-ttu-id="065ab-113">使用 Azure AD 注册应用。</span><span class="sxs-lookup"><span data-stu-id="065ab-113">Register your app with Azure AD.</span></span> 
2. <span data-ttu-id="065ab-114">获取授权。</span><span class="sxs-lookup"><span data-stu-id="065ab-114">Get authorization.</span></span> 
3. <span data-ttu-id="065ab-115">获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="065ab-115">Get an access token.</span></span>
4. <span data-ttu-id="065ab-116">使用访问令牌调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="065ab-116">Call Microsoft Graph with the access token.</span></span>
5. <span data-ttu-id="065ab-117">使用刷新令牌获取新的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="065ab-117">Use a refresh token to get a new access token.</span></span>

## <a name="1-register-your-app"></a><span data-ttu-id="065ab-118">1.注册你的应用程序</span><span class="sxs-lookup"><span data-stu-id="065ab-118">1. Register your app</span></span>
<span data-ttu-id="065ab-p103">若要使用 Azure v2.0 终结点，必须在 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)注册你的应用。你可以使用 Microsoft 帐户或工作或学校帐户注册应用。</span><span class="sxs-lookup"><span data-stu-id="065ab-p103">To use the Azure v2.0 endpoint, you must register your app at the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/). You can use either a Microsoft account or a work or school account to register an app.</span></span> 

<span data-ttu-id="065ab-p104">以下屏幕截图显示 Web 应用注册示例。![使用密码和隐式授予进行 Web 应用注册。](./images/v2-web-registration.png)</span><span class="sxs-lookup"><span data-stu-id="065ab-p104">The following screenshot shows an example Web app registration. ![Web app registration with password and Implicit Grant.](./images/v2-web-registration.png)</span></span>

<span data-ttu-id="065ab-123">若要配置应用以使用 OAuth 2.0 授权代码授予流程，将需要在注册应用时保存下列值：</span><span class="sxs-lookup"><span data-stu-id="065ab-123">To configure an app to use the OAuth 2.0 authorization code grant flow, you'll need to save the following values when registering the app:</span></span>

- <span data-ttu-id="065ab-124">应用注册门户分配的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="065ab-124">The Application ID assigned by the app registration portal.</span></span>
- <span data-ttu-id="065ab-p105">应用密码，可以是密码，也可以是公钥/私钥对（证书）。对于本机应用，这不是必需的。</span><span class="sxs-lookup"><span data-stu-id="065ab-p105">An Application Secret, either a password or a public/private key pair (certificate). This is not required for native apps.</span></span> 
- <span data-ttu-id="065ab-127">可以让应用接收来自 Azure AD 的响应的重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="065ab-127">A Redirect URL for your app to receive responses from Azure AD.</span></span>

<span data-ttu-id="065ab-128">有关如何使用 Microsoft 应用注册门户配置应用的步骤，请参阅[注册你的应用](./auth-register-app-v2.md)。</span><span class="sxs-lookup"><span data-stu-id="065ab-128">For steps on how to configure an app using the Microsoft App Registration Portal, see [Register your app](./auth-register-app-v2.md).</span></span>

## <a name="2-get-authorization"></a><span data-ttu-id="065ab-129">2.获取授权</span><span class="sxs-lookup"><span data-stu-id="065ab-129">2. Get authorization</span></span>
<span data-ttu-id="065ab-p106">对于许多 OpenID Connect 和 OAuth 2.0 流，获取访问令牌的第一步是将用户重定向到 Azure AD v2.0 `/authorize` 终结点。Azure AD 将允许用户登录并确保其同意应用请求的权限。在授权代码授予流中，一旦获得同意，Azure AD 就会将 authorization_code 返回到应用，它可以在 Azure AD v2.0 `/token` 终结点上兑换为访问令牌。</span><span class="sxs-lookup"><span data-stu-id="065ab-p106">The first step to getting an access token for many OpenID Connect and OAuth 2.0 flows is to redirect the user to the Azure AD v2.0 `/authorize` endpoint. Azure AD will sign the user in and ensure their consent for the permissions your app requests. In the authorization code grant flow, after consent is obtained, Azure AD will return an authorization_code to your app that it can redeem at the Azure AD v2.0 `/token` endpoint for an access token.</span></span>

### <a name="authorization-request"></a><span data-ttu-id="065ab-133">授权请求</span><span class="sxs-lookup"><span data-stu-id="065ab-133">Authorization request</span></span> 
<span data-ttu-id="065ab-134">以下示例显示了对 `/authorize` 终结点的请求示例。</span><span class="sxs-lookup"><span data-stu-id="065ab-134">The following shows an example request to the `/authorize` endpoint.</span></span> 

<span data-ttu-id="065ab-p107">通过 Azure AD v2.0 终结点，使用 `scope` 参数请求权限。在此示例中，所请求的 Microsoft Graph 权限可用于 _User.Read_ 和 _Mail.Read_，这会允许应用读取已登录用户的个人资料和邮件。已请求_脱机\_访问_权限，因此应用可以获取刷新令牌，此令牌可用于在当前令牌过期后获取新的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="065ab-p107">With the Azure AD v2.0 endpoint, permissions are requested using the `scope` parameter. In this example, the Microsoft Graph permissions requested are for _User.Read_ and _Mail.Read_, which will allow the app to read the profile and mail of the signed-in user. The _offline\_access_ permission is requested so that the app can get a refresh token, which it can use to get a new access token when the current one expires.</span></span> 

```
// Line breaks for legibility only

https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize?
client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&response_type=code
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&response_mode=query
&scope=offline_access%20user.read%20mail.read
&state=12345
```
| <span data-ttu-id="065ab-138">参数</span><span class="sxs-lookup"><span data-stu-id="065ab-138">Parameter</span></span> |  | <span data-ttu-id="065ab-139">说明</span><span class="sxs-lookup"><span data-stu-id="065ab-139">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="065ab-140">租户</span><span class="sxs-lookup"><span data-stu-id="065ab-140">tenant</span></span> |<span data-ttu-id="065ab-141">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-141">required</span></span> |<span data-ttu-id="065ab-p108">请求路径中的 `{tenant}` 值可用于控制登录应用程序的用户。允许的值为适用于 Microsoft 帐户和工作或学校帐户的 `common`、仅适用于工作或学校帐户的 `organizations`、仅适用于 Microsoft 帐户的 `consumers` 以及租户标识符（如租户 ID 或域名）。有关详细信息，请参阅[协议基础](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints)。</span><span class="sxs-lookup"><span data-stu-id="065ab-p108">The `{tenant}` value in the path of the request can be used to control who can sign into the application.  The allowed values are `common` for both Microsoft accounts and work or school accounts, `organizations` for work or school accounts only, `consumers` for Microsoft accounts only, and tenant identifiers such as the tenant ID or domain name.  For more detail, see [protocol basics](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints).</span></span> |
| <span data-ttu-id="065ab-145">client_id</span><span class="sxs-lookup"><span data-stu-id="065ab-145">client_id</span></span> |<span data-ttu-id="065ab-146">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-146">required</span></span> |<span data-ttu-id="065ab-147">注册门户 ([apps.dev.microsoft.com](https://apps.dev.microsoft.com/?referrer=https://azure.microsoft.com/documentation/articles&deeplink=/appList)) 分配给应用的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="065ab-147">The Application ID that the registration portal ([apps.dev.microsoft.com](https://apps.dev.microsoft.com/?referrer=https://azure.microsoft.com/documentation/articles&deeplink=/appList)) assigned your app.</span></span> |
| <span data-ttu-id="065ab-148">response_type</span><span class="sxs-lookup"><span data-stu-id="065ab-148">response_type</span></span> |<span data-ttu-id="065ab-149">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-149">required</span></span> |<span data-ttu-id="065ab-150">必须包括授权代码流的 `code`。</span><span class="sxs-lookup"><span data-stu-id="065ab-150">Must include `code` for the authorization code flow.</span></span> |
| <span data-ttu-id="065ab-151">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="065ab-151">redirect_uri</span></span> |<span data-ttu-id="065ab-152">建议</span><span class="sxs-lookup"><span data-stu-id="065ab-152">recommended</span></span> |<span data-ttu-id="065ab-p109">你的应用的 redirect_uri，你可以在其中通过应用发送并接收身份验证响应。它必须完全匹配你在应用注册门户中注册的 redirect_uris 之一，除了它必须采用 URL 编码。对于本机和移动应用，应使用默认值 `https://login.microsoftonline.com/common/oauth2/nativeclient`。</span><span class="sxs-lookup"><span data-stu-id="065ab-p109">The redirect_uri of your app, where authentication responses can be sent and received by your app.  It must exactly match one of the redirect_uris you registered in the app registration portal, except it must be URL encoded.  For native and mobile apps, you should use the default value of `https://login.microsoftonline.com/common/oauth2/nativeclient`.</span></span> |
| <span data-ttu-id="065ab-156">范围</span><span class="sxs-lookup"><span data-stu-id="065ab-156">scope</span></span> |<span data-ttu-id="065ab-157">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-157">required</span></span> |<span data-ttu-id="065ab-p110">由空格分隔的希望用户同意的 Microsoft Graph 权限列表。这还可能包括 OpenID 范围。</span><span class="sxs-lookup"><span data-stu-id="065ab-p110">A space-separated list of the Microsoft Graph permissions that you want the user to consent to. This may also include OpenID scopes.</span></span> |
| <span data-ttu-id="065ab-160">response_mode</span><span class="sxs-lookup"><span data-stu-id="065ab-160">response_mode</span></span> |<span data-ttu-id="065ab-161">建议</span><span class="sxs-lookup"><span data-stu-id="065ab-161">recommended</span></span> |<span data-ttu-id="065ab-p111">指定用于将结果令牌发送回应用的方法。可以是 `query` 或 `form_post`。</span><span class="sxs-lookup"><span data-stu-id="065ab-p111">Specifies the method that should be used to send the resulting token back to your app.  Can be `query` or `form_post`.</span></span> |
| <span data-ttu-id="065ab-164">状态</span><span class="sxs-lookup"><span data-stu-id="065ab-164">state</span></span> |<span data-ttu-id="065ab-165">建议</span><span class="sxs-lookup"><span data-stu-id="065ab-165">recommended</span></span> |<span data-ttu-id="065ab-p112">请求中包含的值将在令牌响应中返回。它可以是你希望的任何内容的字符串。随机生成的唯一值通常用于[防止跨网站请求伪造攻击](https://tools.ietf.org/html/rfc6749#section-10.12)。此状态还用于在发生身份验证请求前，对应用中的用户状态信息进行编码（如它们所在的页面或视图上）。</span><span class="sxs-lookup"><span data-stu-id="065ab-p112">A value included in the request that will also be returned in the token response.  It can be a string of any content that you wish.  A randomly generated unique value is typically used for [preventing cross-site request forgery attacks](https://tools.ietf.org/html/rfc6749#section-10.12).  The state is also used to encode information about the user's state in the app before the authentication request occurred, such as the page or view they were on.</span></span> |

> <span data-ttu-id="065ab-p113">**重要说明**：Microsoft Graph 公开两种类型的权限：应用程序性权限和委派权限。对于已登录用户运行的应用，在 `scope` 参数中请求委派权限。这些权限将已登录用户的特权委派给应用，允许其代表已登录的用户来调用 Microsoft Graph。有关可通过 Microsoft Graph 使用的权限的详细信息，请参阅[权限引用](./permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="065ab-p113">**Important**: Microsoft Graph exposes two kinds of permissions: application and delegated. For apps that run with a signed-in user, you request delegated permissions in the `scope` parameter. These permissions delegate the privileges of the signed-in user to your app, allowing it to act as the signed-in user when making calls to Microsoft Graph. For more detailed information about the permissions available through Microsoft Graph, see the [Permissions reference](./permissions-reference.md).</span></span>
 
### <a name="consent-experience"></a><span data-ttu-id="065ab-174">同意体验</span><span class="sxs-lookup"><span data-stu-id="065ab-174">Consent experience</span></span>

<span data-ttu-id="065ab-p114">在这种情况下，将要求用户输入其凭据以使用 Azure AD 进行身份验证。此 v2.0 终结点还将确保用户已同意 `scope` 查询参数中指示的权限。如果用户并不同意任何这些权限，且管理员此前未代表组织内的所有用户表示同意，Azure AD 将提示用户同意所需权限。</span><span class="sxs-lookup"><span data-stu-id="065ab-p114">At this point, the user will be asked to enter their credentials to authenticate with Azure AD. The v2.0 endpoint will also ensure that the user has consented to the permissions indicated in the `scope` query parameter.  If the user has not consented to any of those permissions and if an administrator has not previously consented on behalf of all users in the organization, Azure AD will ask the user to consent to the required permissions.</span></span>  

<span data-ttu-id="065ab-178">以下是为 Microsoft 帐户呈现的同意对话框示例：</span><span class="sxs-lookup"><span data-stu-id="065ab-178">Here is an example of the consent dialog presented for a Microsoft account:</span></span>

![Microsoft 帐户的同意对话框](./images/v2-consumer-consent.png)

> <span data-ttu-id="065ab-p115">**试一试** 如果你拥有 Microsoft 帐户或 Azure AD 工作或学校帐户，可以通过点击以下链接进行尝试：登录后，浏览器应被重定向到地址栏中有 `code` 的 `https://localhost/myapp/`。</span><span class="sxs-lookup"><span data-stu-id="065ab-p115">**Try** If you have a Microsoft account or an Azure AD work or school account, you can try this for yourself by clicking on the link below. After signing in, your browser should be redirected to `https://localhost/myapp/` with a `code` in the address bar.</span></span>
> 
> <span data-ttu-id="065ab-182"><a href="https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&response_type=code&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F&response_mode=query&scope=offline_access%20user.read%20mail.read&state=12345" target="_blank">https://login.microsoftonline.com/common/oauth2/v2.0/authorize...</a></span><span class="sxs-lookup"><span data-stu-id="065ab-182"></span></span>

### <a name="authorization-response"></a><span data-ttu-id="065ab-183">授权响应</span><span class="sxs-lookup"><span data-stu-id="065ab-183">Authorization response</span></span>
<span data-ttu-id="065ab-p116">如果用户同意应用请求的权限，响应将在 `code` 参数中提供授权代码。这是对上述请求的成功响应的示例。因为请求中的 `response_mode` 参数已设为 `query`，响应会在重定向 URL 的查询字符串中返回。</span><span class="sxs-lookup"><span data-stu-id="065ab-p116">If the user consents to the permissions your app requested, the response will contain the authorization code in the `code` parameter. Here is an example of a successful response to the request above. Because the `response_mode` parameter in the request was set to `query`, the response is returned in the query string of the redirect URL.</span></span>

```
GET https://localhost/myapp/?
code=M0ab92efe-b6fd-df08-87dc-2c6500a7f84d
&state=12345
```
| <span data-ttu-id="065ab-187">参数</span><span class="sxs-lookup"><span data-stu-id="065ab-187">Parameter</span></span> | <span data-ttu-id="065ab-188">说明</span><span class="sxs-lookup"><span data-stu-id="065ab-188">Description</span></span> |
| --- | --- |
| <span data-ttu-id="065ab-189">code</span><span class="sxs-lookup"><span data-stu-id="065ab-189">code</span></span> |<span data-ttu-id="065ab-p117">应用请求的 authorization_code。应用可以使用授权代码请求目标资源的访问令牌。Authorization_codes 有效期非常短暂，通常它们会在 10 分钟后失效。</span><span class="sxs-lookup"><span data-stu-id="065ab-p117">The authorization_code that the app requested. The app can use the authorization code to request an access token for the target resource.  Authorization_codes are very short lived, typically they expire after about 10 minutes.</span></span> |
| <span data-ttu-id="065ab-193">状态</span><span class="sxs-lookup"><span data-stu-id="065ab-193">state</span></span> |<span data-ttu-id="065ab-p118">如果请求中包含状态参数，则应在响应中显示相同的值。应用应确认请求和响应中的状态值相同。</span><span class="sxs-lookup"><span data-stu-id="065ab-p118">If a state parameter is included in the request, the same value should appear in the response. The app should verify that the state values in the request and response are identical.</span></span> |

## <a name="3-get-a-token"></a><span data-ttu-id="065ab-196">3.获取令牌</span><span class="sxs-lookup"><span data-stu-id="065ab-196">3. Get a token</span></span>
<span data-ttu-id="065ab-197">你的应用使用上一步接收的授权 `code`，通过发送 `POST` 请求到 `/token` 终结点来请求访问令牌。</span><span class="sxs-lookup"><span data-stu-id="065ab-197">Your app uses the authorization `code` received in the previous step to request an access token by sending a `POST` request to the `/token` endpoint.</span></span>

### <a name="token-request"></a><span data-ttu-id="065ab-198">令牌请求</span><span class="sxs-lookup"><span data-stu-id="065ab-198">Token request</span></span>
```
// Line breaks for legibility only

POST /common/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&code=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq3n8b2JRLk4OxVXr...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=authorization_code
&client_secret=JqQX2PNo9bpM0uEihUPzyrh    // NOTE: Only required for web apps
```

| <span data-ttu-id="065ab-199">参数</span><span class="sxs-lookup"><span data-stu-id="065ab-199">Parameter</span></span> |  | <span data-ttu-id="065ab-200">说明</span><span class="sxs-lookup"><span data-stu-id="065ab-200">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="065ab-201">租户</span><span class="sxs-lookup"><span data-stu-id="065ab-201">tenant</span></span> |<span data-ttu-id="065ab-202">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-202">required</span></span> |<span data-ttu-id="065ab-p119">请求路径中的 `{tenant}` 值可用于控制登录应用程序的用户。允许的值为适用于 Microsoft 帐户和工作或学校帐户的 `common`、仅适用于工作或学校帐户的 `organizations`、仅适用于 Microsoft 帐户的 `consumers` 以及租户标识符（如租户 ID 或域名）。有关详细信息，请参阅[协议基础](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints)。</span><span class="sxs-lookup"><span data-stu-id="065ab-p119">The `{tenant}` value in the path of the request can be used to control who can sign into the application.  The allowed values are `common` for both Microsoft accounts and work or school accounts, `organizations` for work or school accounts only, `consumers` for Microsoft accounts only, and tenant identifiers such as the tenant ID or domain name.  For more detail, see [protocol basics](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints).</span></span> |
| <span data-ttu-id="065ab-206">client_id</span><span class="sxs-lookup"><span data-stu-id="065ab-206">client_id</span></span> |<span data-ttu-id="065ab-207">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-207">required</span></span> |<span data-ttu-id="065ab-208">注册门户 ([apps.dev.microsoft.com](https://apps.dev.microsoft.com/?referrer=https://azure.microsoft.com/documentation/articles&deeplink=/appList)) 分配给应用的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="065ab-208">The Application ID that the registration portal ([apps.dev.microsoft.com](https://apps.dev.microsoft.com/?referrer=https://azure.microsoft.com/documentation/articles&deeplink=/appList)) assigned your app.</span></span> |
| <span data-ttu-id="065ab-209">grant_type</span><span class="sxs-lookup"><span data-stu-id="065ab-209">grant_type</span></span> |<span data-ttu-id="065ab-210">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-210">required</span></span> |<span data-ttu-id="065ab-211">对于授权代码流必须为 `authorization_code`。</span><span class="sxs-lookup"><span data-stu-id="065ab-211">Must be `authorization_code` for the authorization code flow.</span></span> |
| <span data-ttu-id="065ab-212">范围</span><span class="sxs-lookup"><span data-stu-id="065ab-212">scope</span></span> |<span data-ttu-id="065ab-213">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-213">required</span></span> |<span data-ttu-id="065ab-p120">用空格分隔的范围列表。在此图例中请求的范围必须等于在首个（授权）图例中请求的范围或其子集。如果此请求中指定的范围跨越多个资源服务器，则 v2.0 将为首个范围中指定的资源返回令牌。</span><span class="sxs-lookup"><span data-stu-id="065ab-p120">A space-separated list of scopes.  The scopes requested in this leg must be equivalent to or a subset of the scopes requested in the first (authorization) leg.  If the scopes specified in this request span multiple resource servers, then the v2.0 endpoint will return a token for the resource specified in the first scope.</span></span> |
| <span data-ttu-id="065ab-217">code</span><span class="sxs-lookup"><span data-stu-id="065ab-217">code</span></span> |<span data-ttu-id="065ab-218">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-218">required</span></span> |<span data-ttu-id="065ab-219">你在流程的第一个图例中获得的 authorization_code。</span><span class="sxs-lookup"><span data-stu-id="065ab-219">The authorization_code that you acquired in the first leg of the flow.</span></span> |
| <span data-ttu-id="065ab-220">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="065ab-220">redirect_uri</span></span> |<span data-ttu-id="065ab-221">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-221">required</span></span> |<span data-ttu-id="065ab-222">用于获取 authorization_code 的相同的 redirect_uri 值。</span><span class="sxs-lookup"><span data-stu-id="065ab-222">The same redirect_uri value that was used to acquire the authorization_code.</span></span> |
| <span data-ttu-id="065ab-223">client_secret</span><span class="sxs-lookup"><span data-stu-id="065ab-223">client_secret</span></span> |<span data-ttu-id="065ab-224">Web 应用需要</span><span class="sxs-lookup"><span data-stu-id="065ab-224">required for web apps</span></span> |<span data-ttu-id="065ab-p121">你在应用注册门户中为应用创建的应用程序密码。它不可在本机应用中使用，因为设备无法可靠地存储 client_secrets。Web 应用和 Web API 需要此值，它们能够将 client_secret 安全地存储在服务器端上。</span><span class="sxs-lookup"><span data-stu-id="065ab-p121">The application secret that you created in the app registration portal for your app.  It should not be used in a native app, because client_secrets cannot be reliably stored on devices.  It is required for web apps and web APIs, which have the ability to store the client_secret securely on the server side.</span></span> |

### <a name="token-response"></a><span data-ttu-id="065ab-228">令牌响应</span><span class="sxs-lookup"><span data-stu-id="065ab-228">Token response</span></span>
<span data-ttu-id="065ab-229">尽管访问令牌对应用是不透明的，但是响应包含了权限列表，访问令牌对 `scope` 参数中的这些权限有益。</span><span class="sxs-lookup"><span data-stu-id="065ab-229">Although the access token is opaque to your app, the response contains a list of the permissions that the access token is good for in the `scope` parameter.</span></span> 

```
{
    "token_type": "Bearer",
    "scope": "user.read%20Fmail.read",
    "expires_in": 3600,
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik5HVEZ2ZEstZnl0aEV1Q...",
    "refresh_token": "AwABAAAAvPM1KaPlrEqdFSBzjqfTGAMxZGUTdM0t4B4..."
}
```
| <span data-ttu-id="065ab-230">参数</span><span class="sxs-lookup"><span data-stu-id="065ab-230">Parameter</span></span> | <span data-ttu-id="065ab-231">说明</span><span class="sxs-lookup"><span data-stu-id="065ab-231">Description</span></span> |
| --- | --- |
| <span data-ttu-id="065ab-232">token_type</span><span class="sxs-lookup"><span data-stu-id="065ab-232">token_type</span></span> |<span data-ttu-id="065ab-p122">表示令牌类型值。Azure AD 唯一支持的类型是 Bearer</span><span class="sxs-lookup"><span data-stu-id="065ab-p122">Indicates the token type value. The only type that Azure AD supports is Bearer</span></span> |
| <span data-ttu-id="065ab-235">范围</span><span class="sxs-lookup"><span data-stu-id="065ab-235">scope</span></span> |<span data-ttu-id="065ab-236">此 access_token 适用的空格分隔的 Microsoft Graph 权限列表。</span><span class="sxs-lookup"><span data-stu-id="065ab-236">A space separated list of the Microsoft Graph permissions that the access_token is valid for.</span></span> |
| <span data-ttu-id="065ab-237">expires_in</span><span class="sxs-lookup"><span data-stu-id="065ab-237">expires_in</span></span> |<span data-ttu-id="065ab-238">访问令牌的有效期是多久（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="065ab-238">How long the access token is valid (in seconds).</span></span> |
| <span data-ttu-id="065ab-239">access_token</span><span class="sxs-lookup"><span data-stu-id="065ab-239">access_token</span></span> |<span data-ttu-id="065ab-p123">请求的访问令牌。你的应用可以使用此令牌调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="065ab-p123">The requested access token. Your app can use this token to call Microsoft Graph.</span></span> |
| <span data-ttu-id="065ab-242">refresh_token</span><span class="sxs-lookup"><span data-stu-id="065ab-242">refresh_token</span></span> |<span data-ttu-id="065ab-243">OAuth 2.0 刷新令牌。</span><span class="sxs-lookup"><span data-stu-id="065ab-243">An OAuth 2.0 refresh token.</span></span> <span data-ttu-id="065ab-244">在当前访问令牌到期后，应用程序可以使用此令牌获取其他访问令牌。</span><span class="sxs-lookup"><span data-stu-id="065ab-244">Your app can use this token to acquire additional access tokens after the current access token expires.</span></span>  <span data-ttu-id="065ab-245">刷新令牌有效期较长，可用于长时间保留对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="065ab-245">Refresh tokens are long-lived, and can be used to retain access to resources for extended periods of time.</span></span>  <span data-ttu-id="065ab-246">有关详细信息，请参阅 [v2.0 令牌参考](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-tokens)。</span><span class="sxs-lookup"><span data-stu-id="065ab-246">For more detail, refer to the [v2.0 token reference](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-tokens).</span></span> |

## <a name="4-use-the-access-token-to-call-microsoft-graph"></a><span data-ttu-id="065ab-247">4. 使用访问令牌调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="065ab-247">4. Use the access token to call Microsoft Graph</span></span>

<span data-ttu-id="065ab-p125">一旦拥有访问令牌，可以通过将其包含在请求的 `Authorization` 标头中，用其调用 Microsoft Graph。以下请求可以获取已登录用户的个人资料。</span><span class="sxs-lookup"><span data-stu-id="065ab-p125">Once you have an access token, you can use it to call Microsoft Graph by including it in the `Authorization` header of a request. The following request gets the profile of the signed-in user.</span></span>

```
GET https://graph.microsoft.com/v1.0/me 
Authorization: Bearer eyJ0eXAiO ... 0X2tnSQLEANnSPHY0gKcgw
Host: graph.microsoft.com

```
<span data-ttu-id="065ab-250">成功的响应将与此类似（一些响应标头已被删除）：</span><span class="sxs-lookup"><span data-stu-id="065ab-250">A successful response will look similar to this (some response headers have been removed):</span></span>

```
HTTP/1.1 200 OK
Content-Type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
request-id: f45d08c0-6901-473a-90f5-7867287de97f
client-request-id: f45d08c0-6901-473a-90f5-7867287de97f
OData-Version: 4.0
Duration: 727.0022
Date: Thu, 20 Apr 2017 05:21:18 GMT
Content-Length: 407

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

## <a name="5-use-the-refresh-token-to-get-a-new-access-token"></a><span data-ttu-id="065ab-251">5.使用此刷新令牌获取新的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="065ab-251">5. Use the refresh token to get a new access token</span></span>

<span data-ttu-id="065ab-p126">访问令牌有效期非常短暂，在过期后继续访问资源，必须进行刷新。你可以通过向 `/token` 终结点提交其他 `POST` 请求执行此操作，这时提交的是 `refresh_token` 而非 `code`。</span><span class="sxs-lookup"><span data-stu-id="065ab-p126">Access tokens are short lived, and you must refresh them after they expire to continue accessing resources.  You can do so by submitting another `POST` request to the `/token` endpoint, this time providing the `refresh_token` instead of the `code`.</span></span>

### <a name="request"></a><span data-ttu-id="065ab-254">请求</span><span class="sxs-lookup"><span data-stu-id="065ab-254">Request</span></span>
```
// Line breaks for legibility only

POST /common/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&refresh_token=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=refresh_token
&client_secret=JqQX2PNo9bpM0uEihUPzyrh      // NOTE: Only required for web apps
```

| <span data-ttu-id="065ab-255">参数</span><span class="sxs-lookup"><span data-stu-id="065ab-255">Parameter</span></span> |  | <span data-ttu-id="065ab-256">说明</span><span class="sxs-lookup"><span data-stu-id="065ab-256">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="065ab-257">client_id</span><span class="sxs-lookup"><span data-stu-id="065ab-257">client_id</span></span> |<span data-ttu-id="065ab-258">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-258">required</span></span> |<span data-ttu-id="065ab-259">注册门户 ([apps.dev.microsoft.com](https://apps.dev.microsoft.com/?referrer=https://azure.microsoft.com/documentation/articles&deeplink=/appList)) 分配给应用的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="065ab-259">The Application ID that the registration portal ([apps.dev.microsoft.com](https://apps.dev.microsoft.com/?referrer=https://azure.microsoft.com/documentation/articles&deeplink=/appList)) assigned your app.</span></span> |
| <span data-ttu-id="065ab-260">grant_type</span><span class="sxs-lookup"><span data-stu-id="065ab-260">grant_type</span></span> |<span data-ttu-id="065ab-261">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-261">required</span></span> |<span data-ttu-id="065ab-262">必须是 `refresh_token`。</span><span class="sxs-lookup"><span data-stu-id="065ab-262">Must be `refresh_token`.</span></span> |
| <span data-ttu-id="065ab-263">范围</span><span class="sxs-lookup"><span data-stu-id="065ab-263">scope</span></span> |<span data-ttu-id="065ab-264">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-264">required</span></span> |<span data-ttu-id="065ab-p127">用空格分隔的权限列表（范围）。请求的权限必须等于初始 authorization_code 请求中所请求的权限或其子集。</span><span class="sxs-lookup"><span data-stu-id="065ab-p127">A space-separated list of permissions (scopes).  The permissions requested must be equivalent to or a subset of the permissions requested in the original authorization_code request.</span></span> |
| <span data-ttu-id="065ab-267">refresh_token</span><span class="sxs-lookup"><span data-stu-id="065ab-267">refresh_token</span></span> |<span data-ttu-id="065ab-268">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-268">required</span></span> |<span data-ttu-id="065ab-269">令牌请求期间获得的 refresh_token。</span><span class="sxs-lookup"><span data-stu-id="065ab-269">The refresh_token that you acquired during the token request.</span></span> |
| <span data-ttu-id="065ab-270">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="065ab-270">redirect_uri</span></span> |<span data-ttu-id="065ab-271">必需</span><span class="sxs-lookup"><span data-stu-id="065ab-271">required</span></span> |<span data-ttu-id="065ab-272">用于获取 authorization_code 的相同的 redirect_uri 值。</span><span class="sxs-lookup"><span data-stu-id="065ab-272">The same redirect_uri value that was used to acquire the authorization_code.</span></span> |
| <span data-ttu-id="065ab-273">client_secret</span><span class="sxs-lookup"><span data-stu-id="065ab-273">client_secret</span></span> |<span data-ttu-id="065ab-274">Web 应用需要</span><span class="sxs-lookup"><span data-stu-id="065ab-274">required for web apps</span></span> |<span data-ttu-id="065ab-p128">你在应用注册门户中为应用创建的应用程序密码。它不可在本机应用中使用，因为设备无法可靠地存储 client_secrets。Web 应用和 Web API 需要此值，它们能够将 client_secret 安全地存储在服务器端上。</span><span class="sxs-lookup"><span data-stu-id="065ab-p128">The application secret that you created in the app registration portal for your app.  It should not be used in a native app, because client_secrets cannot be reliably stored on devices.  It is required for web apps and web APIs, which have the ability to store the client_secret securely on the server side.</span></span> |

### <a name="response"></a><span data-ttu-id="065ab-278">响应</span><span class="sxs-lookup"><span data-stu-id="065ab-278">Response</span></span>
<span data-ttu-id="065ab-279">成功的令牌响将与下列内容类似。</span><span class="sxs-lookup"><span data-stu-id="065ab-279">A successful token response will look similar to the following.</span></span>

```
{
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik5HVEZ2ZEstZnl0aEV1Q...",
    "token_type": "Bearer",
    "expires_in": 3599,
    "scope": "user.read%20mail.read",
    "refresh_token": "AwABAAAAvPM1KaPlrEqdFSBzjqfTGAMxZGUTdM0t4B4...",
}
```
| <span data-ttu-id="065ab-280">参数</span><span class="sxs-lookup"><span data-stu-id="065ab-280">Parameter</span></span> | <span data-ttu-id="065ab-281">说明</span><span class="sxs-lookup"><span data-stu-id="065ab-281">Description</span></span> |
| --- | --- |
| <span data-ttu-id="065ab-282">access_token</span><span class="sxs-lookup"><span data-stu-id="065ab-282">access_token</span></span> |<span data-ttu-id="065ab-p129">请求的访问令牌。应用可使用此令牌调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="065ab-p129">The requested access token. The app can use this token in calls to Microsoft Graph.</span></span> |
| <span data-ttu-id="065ab-285">token_type</span><span class="sxs-lookup"><span data-stu-id="065ab-285">token_type</span></span> |<span data-ttu-id="065ab-p130">表示令牌类型值。Azure AD 唯一支持的类型是 Bearer</span><span class="sxs-lookup"><span data-stu-id="065ab-p130">Indicates the token type value. The only type that Azure AD supports is Bearer</span></span> |
| <span data-ttu-id="065ab-288">expires_in</span><span class="sxs-lookup"><span data-stu-id="065ab-288">expires_in</span></span> |<span data-ttu-id="065ab-289">访问令牌的有效期是多久（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="065ab-289">How long the access token is valid (in seconds).</span></span> |
| <span data-ttu-id="065ab-290">范围</span><span class="sxs-lookup"><span data-stu-id="065ab-290">scope</span></span> |<span data-ttu-id="065ab-291">access_token 适用的权限（范围）。</span><span class="sxs-lookup"><span data-stu-id="065ab-291">The permissions (scopes) that the access_token is valid for.</span></span> |
| <span data-ttu-id="065ab-292">refresh_token</span><span class="sxs-lookup"><span data-stu-id="065ab-292">refresh_token</span></span> |<span data-ttu-id="065ab-p131">新的 OAuth 2.0 刷新令牌。应当使用刚获得的刷新令牌替换旧的刷新令牌，尽可能确保你的刷新令牌仍旧有效。</span><span class="sxs-lookup"><span data-stu-id="065ab-p131">A new OAuth 2.0 refresh token. You should replace the old refresh token with this newly acquired refresh token to ensure your refresh tokens remain valid for as long as possible.</span></span> |

## <a name="supported-app-scenarios-and-additional-resources"></a><span data-ttu-id="065ab-295">受支持的应用场景和其他资源</span><span class="sxs-lookup"><span data-stu-id="065ab-295">Supported app scenarios and additional resources</span></span>
<span data-ttu-id="065ab-296">你可以代表用户从以下类型的应用中调用 Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="065ab-296">You can call Microsoft Graph on behalf of a user from the following kinds of apps:</span></span> 

- <span data-ttu-id="065ab-297">本机/移动应用</span><span class="sxs-lookup"><span data-stu-id="065ab-297">Native/Mobile apps</span></span> 
- <span data-ttu-id="065ab-298">Web 应用</span><span class="sxs-lookup"><span data-stu-id="065ab-298">Web apps</span></span>
- <span data-ttu-id="065ab-299">单页应用 (SPA)</span><span class="sxs-lookup"><span data-stu-id="065ab-299">Single page apps (SPA)</span></span>
- <span data-ttu-id="065ab-p132">后端 Web API：例如，在如本机应用这样的客户端应用场景中，实现 Web API 后端中的功能。使用 Azure AD v2.0 终结点，客户端应用和后端 Web API 必须都具有相同的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="065ab-p132">Back-end Web APIs: For example, in scenarios where a client app, like a native app, implements functionality in a Web API back end. With the Azure AD v2.0 endpoint, both the client app and the back-end Web API must have the same Application ID.</span></span> 

<span data-ttu-id="065ab-302">有关使用 Azure AD v2.0 终结点的受支持的应用类型的详细信息，请参阅[应用类型](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-flows)。</span><span class="sxs-lookup"><span data-stu-id="065ab-302">For more information about supported app types with the Azure AD v2.0 endpoint, see [Types of apps](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-flows).</span></span>

> <span data-ttu-id="065ab-p133">**注意**：从[独立 Web API](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations#restrictions-on-app-types) 调用 Microsoft Graph 目前不受 Azure AD v2.0 终结点支持。在这种场景下，你需要使用 Azure AD 终结点。</span><span class="sxs-lookup"><span data-stu-id="065ab-p133">**Note**: Calling Microsoft Graph from a [standalone web API](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations#restrictions-on-app-types) is not currently supported by the Azure AD v2.0 endpoint. For this scenario, you need to use the Azure AD endpoint.</span></span>

<span data-ttu-id="065ab-305">有关代表用户从 Azure AD v2.0 终结点获取对 Microsoft Graph 访问的详细信息：</span><span class="sxs-lookup"><span data-stu-id="065ab-305">For more information about getting access to Microsoft Graph on behalf of a user from the Azure AD v2.0 endpoint:</span></span>

- <span data-ttu-id="065ab-306">有关针对不同类型应用的协议文档和入门文章的链接，请参阅 [Azure AD v2.0 终结点文档](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview)。</span><span class="sxs-lookup"><span data-stu-id="065ab-306">For links to protocol documentation and getting started articles for different kinds of apps, see the [Azure AD v2.0 endpoint documentation](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview).</span></span> 
- <span data-ttu-id="065ab-307">有关身份验证流的详细说明，请参阅 [v2.0 协议](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)。</span><span class="sxs-lookup"><span data-stu-id="065ab-307">For detailed explanations of authentication flows, see [v2.0 protocols](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).</span></span>
- <span data-ttu-id="065ab-308">有关建议的 Microsoft 和第三方身份验证库和 Azure AD v2.0 服务器中间件的详细信息，请参阅 [Azure Active Directory v2.0 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries)。</span><span class="sxs-lookup"><span data-stu-id="065ab-308">For more information about recommended Microsoft and third-party authentication libraries and server middleware for Azure AD v2.0, see [Azure Active Directory v2.0 authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries).</span></span>

## <a name="azure-ad-endpoint-considerations"></a><span data-ttu-id="065ab-309">Azure AD 终结点注意事项</span><span class="sxs-lookup"><span data-stu-id="065ab-309">Azure AD endpoint considerations</span></span>
<span data-ttu-id="065ab-p134">Azure AD 终结点和 Azure AD v2.0 终结点的在使用中存在若干区别。例如：</span><span class="sxs-lookup"><span data-stu-id="065ab-p134">There are several differences between using the Azure AD endpoint and the Azure AD v2.0 endpoint. For example:</span></span>

- <span data-ttu-id="065ab-p135">使用 [Azure 门户](https://portal.azure.com)配置应用。有关使用 Azure 门户配置应用的详细信息，请参阅[将应用程序与 Azure Active Directory 相集成：添加应用程序](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications#adding-an-application)</span><span class="sxs-lookup"><span data-stu-id="065ab-p135">You use the [Azure portal](https://portal.azure.com) to configure your app. For more information about configuring apps with the Azure portal, see [Integrating applications with Azure Active Directory: Adding an application](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications#adding-an-application)</span></span>
- <span data-ttu-id="065ab-314">应用将需要每个平台具有不同的应用程序 ID（客户端 ID）。</span><span class="sxs-lookup"><span data-stu-id="065ab-314">Your app will require a different application ID (client ID) for each platform.</span></span>
- <span data-ttu-id="065ab-315">如果应用为多租户应用，则必须在 [Azure 门户](https://portal.azure.com)中通过显式方式将其配置为多租户。</span><span class="sxs-lookup"><span data-stu-id="065ab-315">If your app is a multi-tenant app, you must explicitly configure it to be multi-tenant at the [Azure portal](https://portal.azure.com).</span></span>
- <span data-ttu-id="065ab-p136">使用 Azure AD 终结点时，应用需要的所有权限必须由开发人员进行配置。Azure AD 终结点不支持动态（增量）同意。</span><span class="sxs-lookup"><span data-stu-id="065ab-p136">With the Azure AD endpoint, all permissions that your app needs must be configured by the developer. The Azure AD endpoint does not support dynamic (incremental) consent.</span></span>
- <span data-ttu-id="065ab-p137">Azure AD 终结点使用授权中的 `resource` 参数和令牌请求，指定其需要权限的资源（如 Microsoft Graph）。终结点不支持 `scope` 参数。</span><span class="sxs-lookup"><span data-stu-id="065ab-p137">The Azure AD endpoint uses a `resource` parameter in authorization and token requests to specify the resource, such as Microsoft Graph, for which it wants permissions. The endpoint does not support the `scope` parameter.</span></span> 
- <span data-ttu-id="065ab-p138">Azure AD 终结点不会公开管理员同意的特定终结点。反之，应用会使用授权请求中的 `prompt=admin_consent` 参数，为组织获取管理员同意。有关详细信息，请参阅[将应用程序与 Azure Active Directory 相集成](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications)中的**在运行时引发 Azure AD 同意框架**。</span><span class="sxs-lookup"><span data-stu-id="065ab-p138">The Azure AD endpoint does not expose a specific endpoint for administrator consent. Instead apps use the `prompt=admin_consent` parameter in the authorization request to obtain administrator consent for an organization. For more information, see **Triggering the Azure AD consent framework at runtime** in [Integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications).</span></span>

<span data-ttu-id="065ab-323">有关代表用户从 Azure AD 终结点获取对 Microsoft Graph 访问的详细信息：</span><span class="sxs-lookup"><span data-stu-id="065ab-323">For more information about getting access to Microsoft Graph on behalf of a user from the Azure AD endpoint:</span></span>

- <span data-ttu-id="065ab-p139">有关将 Azure AD 与不同类型的应用结合使用的信息，请参阅 [Azure Active Directory 开发人员指南](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide)中的**入门**链接。该指南包含概述主题、代码演练和 Azure AD 终结点支持的不同类型的应用的协议文档的链接。</span><span class="sxs-lookup"><span data-stu-id="065ab-p139">For information about using the Azure AD endpoint with different kinds of apps, see the **Get Started** links in the [Azure Active Directory developers guide](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide). The guide contains links to overview topics, code walk-throughs, and protocol documentation for different kinds of app supported by the Azure AD endpoint.</span></span>
- <span data-ttu-id="065ab-326">有关 Active Directory 身份验证库 (ADAL) 以及可与 Azure AD 终结点结合使用的服务器中间件的详细信息，请参阅 [Azure Active Directory 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)。</span><span class="sxs-lookup"><span data-stu-id="065ab-326">For information about the Active Directory Authentication Library (ADAL) and server middleware available for use with the Azure AD endpoint, see [Azure Active Directory Authentication Libraries](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).</span></span>

