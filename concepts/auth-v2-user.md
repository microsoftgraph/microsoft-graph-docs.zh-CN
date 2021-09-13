---
title: 代表用户获取访问
description: 若要代表用户使用 Microsoft Graph 读取和写入资源，应用必须从 Azure AD 获取访问令牌，并将令牌附加到其发往 Microsoft Graph 的请求。
author: jackson-woods
ms.localizationpriority: high
ms.prod: applications
ms.custom: graphiamtop20
ms.openlocfilehash: 21c8bf9fb42dc86a149f03adac1bebef3262a233
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59122948"
---
# <a name="get-access-on-behalf-of-a-user"></a>代表用户获取访问权限

若要代表用户使用 Microsoft Graph 读取和写入资源，应用必须从 Microsoft 标识平台获取访问令牌，并将令牌附加到其发往 Microsoft Graph 的请求。你将用于获取访问令牌的确切的身份验证流会依赖于你正在开发的应用类型以及你是否要使用 OpenID Connect 让用户登录到应用中。本机和移动应用还有某些 Web 应用使用的常见流程就是 OAuth 2.0 授权代码授予流程。本主题将介绍一个使用此流程的示例。

## <a name="authentication-and-authorization-steps"></a>身份验证和授权步骤

需要执行下述基本步骤来使用 OAuth 2.0 授权代码授予流从 Microsoft 标识平台终结点获取访问令牌：

1. 使用 Azure AD 注册应用。
2. 获取授权。
3. 获取访问令牌。
4. 使用访问令牌调用 Microsoft Graph。
5. 使用刷新令牌获取新的访问令牌。

## <a name="1-register-your-app"></a>1.注册你的应用程序

要使用 Microsoft 标识平台终结点，必须通过[应用注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)注册应用。可使用 Microsoft 帐户或工作/学校帐户来注册应用。

若要配置应用以使用 OAuth 2.0 授权代码授予流程，将需要在注册应用时保存下列值：

- 应用注册门户分配的应用程序（客户端）ID。
- 客户端（应用）密码，可以是密码，也可以是公钥/私钥对（证书）。对于本机应用，这不是必需的。
- 可让应用接收来自 Azure AD 的响应的重定向 URL（或回复 URL）。

要分步了解如何在 Azure 门户中配置应用，请参阅[注册应用](./auth-register-app-v2.md)。

## <a name="2-get-authorization"></a>2. 获取授权

对于许多 OpenID Connect 和 OAuth 2.0 流，获取访问令牌的第一步是将用户重定向到 Microsoft 标识平台 `/authorize` 端点。Azure AD 将允许用户登录并确保其同意应用请求的权限。在授权代码授予流中，一旦获得同意，Azure AD 就会将 authorization_code 返回到应用，它可以在 Microsoft 标识平台 `/token` 端点上兑换为访问令牌。

### <a name="authorization-request"></a>授权请求

以下示例显示了对 `/authorize` 终结点的请求示例。

通过 Microsoft 标识平台端点，使用 `scope` 参数请求权限。在此示例中，所请求的 Microsoft Graph 权限可用于 _User.Read_ 和 _Mail.Read_，这会允许应用读取已登录用户的个人资料和邮件。已请求 _脱机\_访问_ 权限，因此应用可以获取刷新令牌，此令牌可用于在当前令牌过期后获取新的访问令牌。

```
// Line breaks for legibility only

https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize?
client_id=11111111-1111-1111-1111-111111111111
&response_type=code
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&response_mode=query
&scope=offline_access%20user.read%20mail.read
&state=12345
```

| 参数     | 必需    | 说明                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------|-------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 租户        | 必需    | 请求路径中的 `{tenant}` 值可用于控制登录应用程序的用户。允许的值为适用于 Microsoft 帐户和工作或学校帐户的 `common`、仅适用于工作或学校帐户的 `organizations`、仅适用于 Microsoft 帐户的 `consumers` 以及租户标识符（如租户 ID 或域名）。有关详细信息，请参阅[协议基础](/azure/active-directory/develop/active-directory-v2-protocols#endpoints)。 |
| client_id     | 必需    | [注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)分配给应用的应用程序 ID。                                                                                                                                                                                                                                                                                                                                                                                   |
| response_type | 必需    | 必须包括授权代码流的 `code`。                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| redirect_uri  | 建议 | 你的应用的 redirect_uri，你可以在其中通过应用发送并接收身份验证响应。它必须完全匹配你在应用注册门户中注册的 redirect_uris 之一，除了它必须采用 URL 编码。对于本机和移动应用，应使用默认值 `https://login.microsoftonline.com/common/oauth2/nativeclient`。                                                                                                                                       |
| 范围         | 必需    | 由空格分隔的希望用户同意的 Microsoft Graph 权限列表。 这可能包括资源权限，如 _User.Read_ 和 _Mail.Read_ 和 OIDC 作用域如 `offline_access`，这表示你的应用需要刷新令牌才能长期访问资源。                                                                                                                                                                                                                                                                                                                                                                  |
| response_mode | 建议 | 指定用于将结果令牌发送回应用的方法。可以是 `query` 或 `form_post`。                                                                                                                                                                                                                                                                                                                                                                                  |
| 状态         | 建议 | 请求中包含的值将在令牌响应中返回。它可以是你希望的任何内容的字符串。随机生成的唯一值通常用于[防止跨网站请求伪造攻击](https://tools.ietf.org/html/rfc6749#section-10.12)。此状态还用于在发生身份验证请求前，对应用中的用户状态信息进行编码（如它们所在的页面或视图上）。                                     |

> [!NOTE]
> Microsoft Graph 公开两种类型的权限：应用程序和委派。对于使用已登录用户运行的应用，在 `scope` 参数中请求权限。这些权限将已登录用户的权限委派给您的应用程序，从而允许它在调用 Microsoft Graph 时作为已登录的用户。有关通过 Microsoft Graph 提供的权限的更多详细信息，请参阅 [权限引用](./permissions-reference.md)。
>
> Microsoft Graph 还会公开以下定义明确的 OIDC 作用域： `openid`、 `email`、 `profile`和 `offline_access`。 不支持`address`和`phone` OIDC 作用域。 有关每个 OIDC 作用域的更多详细信息，请参阅 [许可和同意](/azure/active-directory/develop/v2-permissions-and-consent#openid-connect-scopes)。

### <a name="consent-experience"></a>同意体验

在这种情况下，将要求用户输入其凭据以使用 Microsoft 进行身份验证。Microsoft 标识平台 v2.0 端点还将确保用户已同意 `scope` 查询参数中指示的权限。如果用户并不同意任何这些权限，且管理员此前未代表组织内的所有用户表示同意，Azure AD 将提示用户同意所需权限。

下面是为 Microsoft 帐户用户呈现的同意对话框示例。

![Microsoft 帐户的同意对话框](./images/v2-consumer-consent.png)

> **试一试** 如果你拥有 Microsoft 帐户或 Azure AD 工作或学校帐户，可以通过点击以下链接进行尝试：登录后，浏览器应被重定向到地址栏中有 `code` 的 `https://localhost/myapp/`。
>
> <a href="https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&response_type=code&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F&response_mode=query&scope=offline_access%20user.read%20mail.read&state=12345" target="_blank">https://login.microsoftonline.com/common/oauth2/v2.0/authorize...</a>

### <a name="authorization-response"></a>授权响应

如果用户同意应用请求的权限，响应将在 `code` 参数中提供授权代码。这是对上述请求的成功响应的示例。因为请求中的 `response_mode` 参数已设为 `query`，响应会在重定向 URL 的查询字符串中返回。

```
GET https://localhost/myapp/?
code=M0ab92efe-b6fd-df08-87dc-2c6500a7f84d
&state=12345
```

| 参数 | 说明                                                                                                                                                                                                                        |
|-----------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| code      | 应用请求的 authorization_code。应用可以使用授权代码请求目标资源的访问令牌。Authorization_codes 有效期非常短暂，通常它们会在 10 分钟后失效。 |
| 状态     | 如果请求中包含状态参数，则应在响应中显示相同的值。应用应确认请求和响应中的状态值相同。                                              |

## <a name="3-get-a-token"></a>3.获取令牌

你的应用使用上一步接收的授权 `code`，通过发送 `POST` 请求到 `/token` 终结点来请求访问令牌。

### <a name="token-request"></a>令牌请求

```
// Line breaks for legibility only

POST /{tenant}/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=11111111-1111-1111-1111-111111111111
&scope=user.read%20mail.read
&code=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq3n8b2JRLk4OxVXr...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=authorization_code
&client_secret=jXoM3iz...    // NOTE: Only required for web apps
```

| 参数     | 必需              | 说明                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 租户        | 必需              | 请求路径中的 `{tenant}` 值可用于控制登录应用程序的用户。允许的值为适用于 Microsoft 帐户和工作或学校帐户的 `common`、仅适用于工作或学校帐户的 `organizations`、仅适用于 Microsoft 帐户的 `consumers` 以及租户标识符（如租户 ID 或域名）。有关详细信息，请参阅[协议基础](/azure/active-directory/develop/active-directory-v2-protocols#endpoints)。 |
| client_id     | 必需              | [注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)分配给应用的应用程序 ID。                                                                                                                                                                                                                                                                                                                                                                                  |
| grant_type    | 必需              | 对于授权代码流必须为 `authorization_code`。                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| 范围         | 必需              | 用空格分隔的范围列表。在此图例中请求的范围必须等于在首个（授权）图例中请求的范围或其子集。如果此请求中指定的范围跨越多个资源服务器，则 v2.0 将为首个范围中指定的资源返回令牌。                                                                                                                                                                      |
| code          | 必需              | 你在流程的第一个图例中获得的 authorization_code。                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| redirect_uri  | 必需              | 用于获取 authorization_code 的相同的 redirect_uri 值。                                                                                                                                                                                                                                                                                                                                                                                                                            |
| client_secret | Web 应用需要 | 你在应用注册门户中为应用创建的应用程序密码。它不可在本机应用中使用，因为设备无法可靠地存储 client_secrets。Web 应用和 Web API 需要此值，它们能够将 client_secret 安全地存储在服务器端上。                                                                                                                                                                                     |

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
| token_type    | 表示令牌类型值。Azure AD 唯一支持的类型是 Bearer。                                                                                                                                                                                                                                                                                                              |
| 范围         | 此 access_token 适用的空格分隔的 Microsoft Graph 权限列表。                                                                                                                                                                                                                                                                                                |
| expires_in    | 访问令牌的有效期是多久（以秒为单位）。                                                                                                                                                                                                                                                                                                                                             |
| access_token  | 请求的访问令牌。你的应用可以使用此令牌调用 Microsoft Graph。                                                                                                                                                                                                                                                                                                             |
| refresh_token | OAuth 2.0 刷新令牌。 在当前访问令牌到期后，应用程序可以使用此令牌获取其他访问令牌。  刷新令牌有效期较长，可用于长时间保留对资源的访问权限。  有关详细信息，请参阅 [v2.0 令牌参考](/azure/active-directory/develop/active-directory-v2-tokens)。 |

## <a name="4-use-the-access-token-to-call-microsoft-graph"></a>4. 使用访问令牌调用 Microsoft Graph

拥有访问令牌后，可通过将其包含在请求的 `Authorization` 标头中，用其调用 Microsoft Graph。以下请求可获取已登录用户的个人资料。

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

访问令牌有效期非常短暂，在过期后继续访问资源，必须进行刷新。你可以通过向 `/token` 终结点提交其他 `POST` 请求执行此操作，这时提交的是 `refresh_token` 而非 `code`。

### <a name="request"></a>请求

```
// Line breaks for legibility only

POST /common/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=11111111-1111-1111-1111-111111111111
&scope=user.read%20mail.read
&refresh_token=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=refresh_token
&client_secret=jXoM3iz...      // NOTE: Only required for web apps
```

| 参数     | 必需              | 说明                                                                                                                                                                                                                                                                                                         |
|---------------|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client_id     | 必需              | [注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)分配给应用的应用程序 ID。                                                                                                                                                                                               |
| grant_type    | 必需              | 必须是 `refresh_token`。                                                                                                                                                                                                                                                                                            |
| 范围         | 必需              | 用空格分隔的权限列表（范围）。请求的权限必须等于初始 authorization_code 请求中所请求的权限或其子集。                                                                                                                               |
| refresh_token | 必需              | 令牌请求期间获得的 refresh_token。                                                                                                                                                                                                                                                       |
| redirect_uri  | 必需              | 用于获取 authorization_code 的相同的 redirect_uri 值。                                                                                                                                                                                                                                        |
| client_secret | Web 应用需要 | 你在应用注册门户中为应用创建的应用程序密码。它不可在本机应用中使用，因为设备无法可靠地存储 client_secrets。Web 应用和 Web API 需要此值，它们能够将 client_secret 安全地存储在服务器端上。 |

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
| access_token  | 请求的访问令牌。应用可使用此令牌调用 Microsoft Graph。                                                                                                |
| token_type    | 表示令牌类型值。Azure AD 唯一支持的类型是 Bearer                                                                                                     |
| expires_in    | 访问令牌的有效期是多久（以秒为单位）。                                                                                                                                   |
| 范围         | access_token 适用的权限（范围）。                                                                                                                       |
| refresh_token | 新的 OAuth 2.0 刷新令牌。应当使用刚获得的刷新令牌替换旧的刷新令牌，尽可能确保你的刷新令牌仍旧有效。 |

## <a name="supported-app-scenarios-and-additional-resources"></a>受支持的应用场景和其他资源

你可以代表用户从以下类型的应用中调用 Microsoft Graph:

- [本机/移动应用](/azure/active-directory/develop/scenario-mobile-overview)
- [Web 应用](/azure/active-directory/develop/scenario-web-app-call-api-overview)
- [单页应用 (SPA)](/azure/active-directory/develop/scenario-spa-overview)
- [后端 Web API](/azure/active-directory/develop/scenario-web-app-call-api-overview)：例如，在如本机应用这样的客户端应用场景中，实现 Web API 后端中的功能。使用 Microsoft 标识平台终结点，客户端应用和后端 Web API 必须都具有相同的应用程序 ID。

要详细了解 Microsoft 标识平台终结点支持的应用方案，请参阅[应用方案和身份验证流程](/azure/active-directory/develop/authentication-flows-app-scenarios)。

> **请注意**: 从独立 Web API 调用 Microsoft Graph 目前不受 Microsoft 标识平台端点支持。在这种场景下，需要使用 Azure AD 端点。

若要详细了解如何代表用户从 Microsoft标识平台终结点获取访问 Microsoft Graph 的权限：

- 有关指向不同类型应用的协议文档和入门文章的链接，请参阅 [Microsoft 标识平台终结点文档](/azure/active-directory/develop/active-directory-appmodel-v2-overview)。
- 要详细了解受支持的应用程序类型和身份验证流程，请参阅 [v2.0 应用类型](/azure/active-directory/develop/v2-app-types)。
- 要详细了解为 Microsoft 标识平台推荐的 Microsoft 和第三方身份验证库及服务器中间件，请参阅 [Azure Active Directory v2.0 身份验证库](/azure/active-directory/develop/active-directory-v2-libraries)。

## <a name="endpoint-considerations"></a>终结点注意事项

Microsoft 继续支持 Azure AD 终结点。 在使用 Microsoft 标识平台终结点和使用 Azure AD 终结点之间存在[诸多区别](/azure/active-directory/develop/azure-ad-endpoint-comparison)。 使用 Azure AD 终结点时：

- 应用将需要为每个平台提供不同的应用程序 ID（客户端 ID）。
- 如果应用为多租户应用，则必须在 [Azure 门户](https://portal.azure.com)中通过显式方式将其配置为多租户。
- 应用需要的所有权限必须由开发人员进行配置。Azure AD 终结点不支持动态（增量）同意。
- Azure AD 终结点使用授权中的 `resource` 参数和令牌请求，指定其需要权限的资源（如 Microsoft Graph）。终结点不支持 `scope` 参数。
- Azure AD 终结点不会公开管理员同意的特定终结点。反之，应用会使用授权请求中的 `prompt=admin_consent` 参数，为组织获取管理员同意。有关详细信息，请参阅 [将应用程序与 Azure Active Directory 相集成](/azure/active-directory/develop/active-directory-integrating-applications)中的 **在运行时引发 Azure AD 同意框架**。

有关代表用户从 Azure AD 终结点获取对 Microsoft Graph 访问的详细信息：

- 要了解如何将 Microsoft 标识平台终结点与不同类型的应用结合使用，请参阅 [Microsoft 标识平台开发人员文档](/azure/active-directory/develop/active-directory-developers-guide)中的 **开始使用** 链接。 该文档包含众多链接，可通过它们查看 Microsoft 标识平台终结点支持的不同类型的应用的概述主题、快速入门、教程、代码示例和协议文档。
- 要了解可与 Microsoft 标识平台终结点结合使用的 Microsoft 身份验证库 (MSAL) 和服务器中间件，请参阅 [Microsoft 身份验证库](/azure/active-directory/develop/msal-overview)。

## <a name="see-also"></a>另请参阅

- 有关 Azure 应用服务上托管的 Web 应用调用 Microsoft Graph 作为用户的示例，请参阅[教程：从安全应用访问作为用户的 Microsoft Graph](/azure/app-service/scenario-secure-app-access-microsoft-graph-as-user)。 了解如何向 Web 应用授予委派权限、配置应用服务以获取访问令牌，以及如何从 Web 应用为登录用户调用 Microsoft Graph。
- 有关使用 Microsoft 标识平台保护不同应用程序类型的示例，请查看 [Microsoft 标识平台代码示例（v2.0 终结点）](/azure/active-directory/develop/sample-v2-code)。
