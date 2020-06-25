---
title: 代表用户获取访问
description: 若要代表用户使用 Microsoft Graph 读取和写入资源，应用必须从 Azure AD 获取访问令牌，并将令牌附加到其发往 Microsoft Graph 的请求。
author: jackson-woods
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: graphiamtop20
ms.openlocfilehash: d2b3c7a26a0a4d5005f22893e0295585f5e7033b
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846154"
---
# <a name="get-access-on-behalf-of-a-user"></a>代表用户获取访问权限

To use Microsoft Graph to read and write resources on behalf of a user, your app must get an access token from the Microsoft identity platform and attach the token to requests that it sends to Microsoft Graph. The exact authentication flow that you will use to get access tokens will depend on the kind of app you are developing and whether you want to use OpenID Connect to sign the user in to your app. One common flow used by native and mobile apps and also by some Web apps is the OAuth 2.0 authorization code grant flow. This topic  walks through an example using this flow.

## <a name="authentication-and-authorization-steps"></a>身份验证和授权步骤

需要执行下述基本步骤来使用 OAuth 2.0 授权代码授予流从 Microsoft 标识平台终结点获取访问令牌：

1. 使用 Azure AD 注册应用。
2. 获取授权。
3. 获取访问令牌。
4. 使用访问令牌调用 Microsoft Graph。
5. 使用刷新令牌获取新的访问令牌。

## <a name="1-register-your-app"></a>1.注册你的应用程序

To use the Microsoft identity platform endpoint, you must register your app using the Azure [app registration portal](https://go.microsoft.com/fwlink/?linkid=2083908). You can use either a Microsoft account or a work or school account to register an app.

若要配置应用以使用 OAuth 2.0 授权代码授予流程，将需要在注册应用时保存下列值：

- 应用注册门户分配的应用程序（客户端）ID。
- 客户端（应用程序）密码，它是一个密码或是一个公钥/私钥对（证书）。 这不是本机应用的必需项。
- 可让应用接收来自 Azure AD 的响应的重定向 URL（或回复 URL）。

要分步了解如何在 Azure 门户中配置应用，请参阅[注册应用](./auth-register-app-v2.md)。

## <a name="2-get-authorization"></a>2. 获取授权

首先是从多个 OpenID Connect 获取访问令牌，然后 OAuth 2.0 流会将用户重定向到 Microsoft 标识平台 `/authorize` 终结点。 Azure AD 将允许用户登录并确保其同意应用请求的权限。 在授权代码授予流中，获得同意后，Azure AD 将向你的应用返回一个授权代码，它可在 Microsoft 标识平台 `/token` 终结点处兑换访问令牌。

### <a name="authorization-request"></a>授权请求

以下示例显示了对 `/authorize` 终结点的请求示例。

借助 Microsoft 标识平台终结点，通过 `scope` 参数请求权限。 在本例中，所请求的 Microsoft Graph 权限可用于 _User.Read_ 和 _Mail.Read_，从而让应用能够读取已登录用户的个人资料和邮件。 已请求_脱机\_访问_权限，这样应用就可获取刷新令牌，后者可用于在当前访问令牌过期时获取新的令牌。

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

| 参数     | 必需    | 说明                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------|-------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 租户        | 必需    | The `{tenant}` value in the path of the request can be used to control who can sign into the application.  The allowed values are `common` for both Microsoft accounts and work or school accounts, `organizations` for work or school accounts only, `consumers` for Microsoft accounts only, and tenant identifiers such as the tenant ID or domain name.  For more detail, see [protocol basics](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints). |
| client_id     | 必需    | [注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)分配给应用的应用程序 ID。                                                                                                                                                                                                                                                                                                                                                                                   |
| response_type | 必需    | 必须包括授权代码流的 `code`。                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| redirect_uri  | 建议 | The redirect_uri of your app, where authentication responses can be sent and received by your app.  It must exactly match one of the redirect_uris you registered in the app registration portal, except it must be URL encoded.  For native and mobile apps, you should use the default value of `https://login.microsoftonline.com/common/oauth2/nativeclient`.                                                                                                                                       |
| 范围         | 必需    | A space-separated list of the Microsoft Graph permissions that you want the user to consent to. This may also include OpenID scopes.                                                                                                                                                                                                                                                                                                                                                                    |
| response_mode | 建议 | Specifies the method that should be used to send the resulting token back to your app.  Can be `query` or `form_post`.                                                                                                                                                                                                                                                                                                                                                                                  |
| 状态         | 建议 | A value included in the request that will also be returned in the token response.  It can be a string of any content that you wish.  A randomly generated unique value is typically used for [preventing cross-site request forgery attacks](https://tools.ietf.org/html/rfc6749#section-10.12).  The state is also used to encode information about the user's state in the app before the authentication request occurred, such as the page or view they were on.                                     |

> **Important**: Microsoft Graph exposes two kinds of permissions: application and delegated. For apps that run with a signed-in user, you request delegated permissions in the `scope` parameter. These permissions delegate the privileges of the signed-in user to your app, allowing it to act as the signed-in user when making calls to Microsoft Graph. For more detailed information about the permissions available through Microsoft Graph, see the [Permissions reference](./permissions-reference.md).

### <a name="consent-experience"></a>同意体验

此时，用户将需要输入其凭据才能向 Microsoft 进行身份验证。 Microsoft 标识平台 v2.0 终结点还将确保用户已同意 `scope` 查询参数中指示的权限。  如果用户未同意上述任何权限，以及管理员之前未代表组织中的所有用户授予同意，则他们需要同意所需权限。

下面是为 Microsoft 帐户用户呈现的同意对话框示例。

![Microsoft 帐户的同意对话框](./images/v2-consumer-consent.png)

> **Try** If you have a Microsoft account or an Azure AD work or school account, you can try this for yourself by clicking the following link. After signing in, your browser should be redirected to `https://localhost/myapp/` with a `code` in the address bar.
>
> <a href="https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&response_type=code&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F&response_mode=query&scope=offline_access%20user.read%20mail.read&state=12345" target="_blank">https://login.microsoftonline.com/common/oauth2/v2.0/authorize...</a>

### <a name="authorization-response"></a>授权响应

If the user consents to the permissions your app requested, the response will contain the authorization code in the `code` parameter. Here is an example of a successful response to the previous request. Because the `response_mode` parameter in the request was set to `query`, the response is returned in the query string of the redirect URL.

```
GET https://localhost/myapp/?
code=M0ab92efe-b6fd-df08-87dc-2c6500a7f84d
&state=12345
```

| 参数 | 说明                                                                                                                                                                                                                        |
|-----------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| code      | The authorization_code that the app requested. The app can use the authorization code to request an access token for the target resource.  Authorization_codes are very short lived, typically they expire after about 10 minutes. |
| 状态     | If a state parameter is included in the request, the same value should appear in the response. The app should verify that the state values in the request and response are identical.                                              |

## <a name="3-get-a-token"></a>3.获取令牌

你的应用使用上一步接收的授权 `code`，通过发送 `POST` 请求到 `/token` 终结点来请求访问令牌。

### <a name="token-request"></a>令牌请求

```
// Line breaks for legibility only

POST /{tenant}/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&code=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq3n8b2JRLk4OxVXr...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=authorization_code
&client_secret=JqQX2PNo9bpM0uEihUPzyrh    // NOTE: Only required for web apps
```

| 参数     | 必需              | 说明                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 租户        | 必需              | The `{tenant}` value in the path of the request can be used to control who can sign into the application.  The allowed values are `common` for both Microsoft accounts and work or school accounts, `organizations` for work or school accounts only, `consumers` for Microsoft accounts only, and tenant identifiers such as the tenant ID or domain name.  For more detail, see [protocol basics](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints). |
| client_id     | 必需              | [注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)分配给应用的应用程序 ID。                                                                                                                                                                                                                                                                                                                                                                                  |
| grant_type    | 必需              | 对于授权代码流必须为 `authorization_code`。                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| 范围         | 必需              | A space-separated list of scopes.  The scopes requested in this leg must be equivalent to or a subset of the scopes requested in the first (authorization) leg.  If the scopes specified in this request span multiple resource servers, then the v2.0 endpoint will return a token for the resource specified in the first scope.                                                                                                                                                                      |
| code          | 必需              | 你在流程的第一个图例中获得的 authorization_code。                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| redirect_uri  | 必需              | 用于获取 authorization_code 的相同的 redirect_uri 值。                                                                                                                                                                                                                                                                                                                                                                                                                            |
| client_secret | Web 应用需要 | The application secret that you created in the app registration portal for your app.  It should not be used in a native app, because client_secrets cannot be reliably stored on devices.  It is required for web apps and web APIs, which have the ability to store the client_secret securely on the server side.                                                                                                                                                                                     |

### <a name="token-response"></a>令牌响应

尽管访问令牌对应用是不透明的，但是响应包含了权限列表，访问令牌对 `scope` 参数中的这些权限有益。

```json
{
    "token_type": "Bearer",
    "scope": "user.read%20Fmail.read",
    "expires_in": 3600,
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik5HVEZ2ZEstZnl0aEV1Q...",
    "refresh_token": "AwABAAAAvPM1KaPlrEqdFSBzjqfTGAMxZGUTdM0t4B4..."
}
```

| 参数     | 说明                                                                                                                                                                                                                                                                                                                                                                                  |
|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| token_type    | Indicates the token type value. The only type that Azure AD supports is Bearer.                                                                                                                                                                                                                                                                                                              |
| 范围         | 此 access_token 适用的空格分隔的 Microsoft Graph 权限列表。                                                                                                                                                                                                                                                                                                |
| expires_in    | 访问令牌的有效期是多久（以秒为单位）。                                                                                                                                                                                                                                                                                                                                             |
| access_token  | The requested access token. Your app can use this token to call Microsoft Graph.                                                                                                                                                                                                                                                                                                             |
| refresh_token | OAuth 2.0 刷新令牌。 在当前访问令牌到期后，应用程序可以使用此令牌获取其他访问令牌。  刷新令牌有效期较长，可用于长时间保留对资源的访问权限。  有关详细信息，请参阅 [v2.0 令牌参考](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-tokens)。 |

## <a name="4-use-the-access-token-to-call-microsoft-graph"></a>4. 使用访问令牌调用 Microsoft Graph

After you have an access token, you can use it to call Microsoft Graph by including it in the `Authorization` header of a request. The following request gets the profile of the signed-in user.

```
GET https://graph.microsoft.com/v1.0/me
Authorization: Bearer eyJ0eXAiO ... 0X2tnSQLEANnSPHY0gKcgw
Host: graph.microsoft.com

```

成功的响应将与下述内容类似（一些响应标头已被删除）。

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

## <a name="5-use-the-refresh-token-to-get-a-new-access-token"></a>5.使用此刷新令牌获取新的访问令牌。

Access tokens are short lived, and you must refresh them after they expire to continue accessing resources.  You can do so by submitting another `POST` request to the `/token` endpoint, this time providing the `refresh_token` instead of the `code`.

### <a name="request"></a>请求

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

| 参数     | 必需              | 说明                                                                                                                                                                                                                                                                                                         |
|---------------|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client_id     | 必需              | [注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)分配给应用的应用程序 ID。                                                                                                                                                                                               |
| grant_type    | 必需              | 必须是 `refresh_token`。                                                                                                                                                                                                                                                                                            |
| 范围         | 必需              | A space-separated list of permissions (scopes).  The permissions requested must be equivalent to or a subset of the permissions requested in the original authorization_code request.                                                                                                                               |
| refresh_token | 必需              | 令牌请求期间获得的 refresh_token。                                                                                                                                                                                                                                                       |
| redirect_uri  | 必需              | 用于获取 authorization_code 的相同的 redirect_uri 值。                                                                                                                                                                                                                                        |
| client_secret | Web 应用需要 | The application secret that you created in the app registration portal for your app.  It should not be used in a native app, because client_secrets cannot be reliably stored on devices.  It is required for web apps and web APIs, which have the ability to store the client_secret securely on the server side. |

### <a name="response"></a>响应

成功的令牌响将与下列内容类似。

```
{
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik5HVEZ2ZEstZnl0aEV1Q...",
    "token_type": "Bearer",
    "expires_in": 3599,
    "scope": "user.read%20mail.read",
    "refresh_token": "AwABAAAAvPM1KaPlrEqdFSBzjqfTGAMxZGUTdM0t4B4...",
}
```
| 参数     | 说明                                                                                                                                                                        |
|---------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| access_token  | The requested access token. The app can use this token in calls to Microsoft Graph.                                                                                                |
| token_type    | Indicates the token type value. The only type that Azure AD supports is Bearer                                                                                                     |
| expires_in    | 访问令牌的有效期是多久（以秒为单位）。                                                                                                                                   |
| 范围         | access_token 适用的权限（范围）。                                                                                                                       |
| refresh_token | A new OAuth 2.0 refresh token. You should replace the old refresh token with this newly acquired refresh token to ensure your refresh tokens remain valid for as long as possible. |

## <a name="supported-app-scenarios-and-additional-resources"></a>受支持的应用场景和其他资源

你可以代表用户从以下类型的应用中调用 Microsoft Graph:

- [本机/移动应用](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-overview)
- [Web 应用](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-call-api-overview)
- [单页应用 (SPA)](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-overview)
- [后端 Web API](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-call-api-overview)：例如，在本机应用等客户端应用在 Web API 后端实现功能的情况下。 通过 Microsoft 标识平台终结点，客户端应用和后端 Web API 必须具有相同的应用程序 ID。

要详细了解 Microsoft 标识平台终结点支持的应用方案，请参阅[应用方案和身份验证流程](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios)。

> **请注意**：Microsoft 标识平台终结点当前不支持通过独立的 Web API 调用 Microsoft Graph。 在此情况下，需要使用 Azure AD 终结点。

若要详细了解如何代表用户从 Microsoft标识平台终结点获取访问 Microsoft Graph 的权限：

- 有关指向不同类型应用的协议文档和入门文章的链接，请参阅 [Microsoft 标识平台终结点文档](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview)。
- 要详细了解受支持的应用程序类型和身份验证流程，请参阅 [v2.0 应用类型](https://docs.microsoft.com/azure/active-directory/develop/v2-app-types)。
- 要详细了解为 Microsoft 标识平台推荐的 Microsoft 和第三方身份验证库及服务器中间件，请参阅 [Azure Active Directory v2.0 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries)。

## <a name="endpoint-considerations"></a>终结点注意事项

Microsoft 继续支持 Azure AD 终结点。 在使用 Microsoft 标识平台终结点和使用 Azure AD 终结点之间存在[诸多区别](https://docs.microsoft.com/azure/active-directory/develop/azure-ad-endpoint-comparison)。 使用 Azure AD 终结点时：

- 应用将需要为每个平台提供不同的应用程序 ID（客户端 ID）。
- 如果应用为多租户应用，则必须在 [Azure 门户](https://portal.azure.com)中通过显式方式将其配置为多租户。
- 应用必需的所有权限都必须由开发人员进行配置。 Azure AD 终结点不支持动态（增量）同意。
- The Azure AD endpoint uses a `resource` parameter in authorization and token requests to specify the resource, such as Microsoft Graph, for which it wants permissions. The endpoint does not support the `scope` parameter.
- The Azure AD endpoint does not expose a specific endpoint for administrator consent. Instead apps use the `prompt=admin_consent` parameter in the authorization request to obtain administrator consent for an organization. For more information, see **Triggering the Azure AD consent framework at runtime** in [Integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications).

有关代表用户从 Azure AD 终结点获取对 Microsoft Graph 访问的详细信息：

- 要了解如何将 Microsoft 标识平台终结点与不同类型的应用结合使用，请参阅 [Microsoft 标识平台开发人员文档](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide)中的**开始使用**链接。 该文档包含众多链接，可通过它们查看 Microsoft 标识平台终结点支持的不同类型的应用的概述主题、快速入门、教程、代码示例和协议文档。
- 要了解可与 Microsoft 标识平台终结点结合使用的 Microsoft 身份验证库 (MSAL) 和服务器中间件，请参阅 [Microsoft 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/msal-overview)。
