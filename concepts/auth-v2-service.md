---
title: 在没有用户的情况下获取访问权限
description: 一些应用使用他们自己的标识（而不代表用户）调用 Microsoft Graph。 在许多情况下，这些是在服务器上运行的后台服务或守护程序，不存在登录用户。
author: jackson-woods
localization_priority: Priority
ms.prod: applications
ms.custom: graphiamtop20
ms.openlocfilehash: 0fba65fb040ca210b5d9a9fe82e9510b5586c4b6
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53333966"
---
# <a name="get-access-without-a-user"></a>在没有用户的情况下获取访问权限

一些应用使用他们自己的标识（而不代表用户）调用 Microsoft Graph。在许多情况下，这些是在的服务器上运行的后台服务或守护程序，不存在登录用户。此类应用的一个示例是电子邮件存档服务，它可以在夜间保持清醒状态并运行。在某些情况下，具有登录用户的应用可能还需要以他们自己的标识调用 Microsoft Graph。例如，应用可能需要使用以下特定功能，该功能要求在组织中具有比登录用户的提升权限更多的权限。  

使用它们自己的标识调用 Microsoft Graph 的应用使用 OAuth 2.0 [客户端凭据授予流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)从 Azure AD 获取访问令牌。本主题介绍了配置服务和使用 OAuth 客户端凭据授予流获取访问令牌的基本步骤。

## <a name="authentication-and-authorization-steps"></a>身份验证和授权步骤

需要执行下列基本步骤来配置服务并从 Microsoft 标识平台终结点获取你的服务在其自身标识下调用 Microsoft Graph 时所用的令牌：

1. 注册应用。
2. 在应用上配置 Microsoft Graph 的权限。
3. 获取管理员同意。
4. 获取访问令牌。
5. 使用访问令牌调用 Microsoft Graph。

## <a name="1-register-your-app"></a>1.注册你的应用程序

要向 Microsoft 标识平台终结点进行身份验证，必须先在 [Azure 应用注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)注册你的应用。你可使用 Microsoft 帐户或工作/学校帐户来注册应用。

对于将以自己的标识调用 Microsoft Graph 的服务，用户需要将应用注册到 Web 平台并复制以下值：

- Azure 应用注册门户分配的应用程序 ID。
- 客户端（应用程序）密码，它是一个密码或是一个公钥/私钥对（证书）。
- 服务用于接收令牌响应的重定向 URL。
- 服务用于接收管理员同意答复的重定向 URL（在你的应用实现功能来请求管理员同意的情况下）。  

要分步了解如何通过 Azure 应用注册门户配置应用，请参阅[注册应用](./auth-register-app-v2.md)。

借助 OAuth 2.0 客户端凭据授予流，你的应用可通过 Azure AD 分配的应用程序 ID 以及依靠门户创建的应用程序密码在 Microsoft 标识平台 `/token` 终结点处直接进行身份验证。

## <a name="2-configure-permissions-for-microsoft-graph"></a>2.配置 Microsoft Graph 的权限

对于以它们自己的标识调用 Microsoft Graph 的应用，Microsoft Graph 显示应用程序权限。（Microsoft Graph 还显示代表用户调用 Microsoft Graph 的应用的委派权限。）注册应用时，需要预配置应用所需的应用程序权限。应用程序权限始终需要管理员的同意。当你的应用安装在他们的组织中时，管理员可以使用 [Azure 门户](https://portal.azure.com)同意这些权限，你也可以提供应用注册体验，让管理员同意你配置的权限。Azure AD 记录管理员同意后，你的应用无需再次请求同意即可请求令牌。有关可通过 Microsoft Graph 使用的权限的详细信息，请参阅[权限参考](./permissions-reference.md)

若要在 [Azure 应用注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)为应用配置应用程序权限：在应用程序的 **API 权限** 页面中，选择“**添加权限**”，选择“**Microsoft Graph**”，然后在“**应用程序权限**”下选择你的应用所需的权限。

下面的屏幕快照显示了 Microsoft Graph 应用程序权限的“**选择权限**”对话框。

![Microsoft Graph 应用程序权限的“选择权限”对话框。](./images/auth-v2/v2-application-permissions.png)

> **注意**：建议配置应用需要的最小特权权限集。这为管理员提供的体验要比不得不同意一个很长的权限列表的体验舒适得多。

## <a name="3-get-administrator-consent"></a>3.获取管理员同意

你可让管理员在 [Azure 门户](https://portal.azure.com)授予你的应用所需的权限；但通常情况下，更好的方法是通过 Microsoft 标识平台 `/adminconsent` 终结点提供管理员注册体验。 

> **重要说明**：任何时候更改配置权限都必须重复管理员同意过程。 租户管理员重新应用同意之后，才会反映应用注册门户中所做的更改。

### <a name="request"></a>请求

```
// Line breaks are for legibility only.

GET https://login.microsoftonline.com/{tenant}/adminconsent
?client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&state=12345
&redirect_uri=https://localhost/myapp/permissions
```

| 参数     | 条件   | 说明 
|:--------------|:------------|:------------
| 租户        | 必需    | 需要从中请求权限的目录租户。它可以 GUID 或友好名称格式显示。如果你不了解用户授予哪个租户，并想让用户使用任意租户登录，请使用 `common`。
| client_id     | 必需    | [Azure 应用注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)分配给你的应用的应用程序 ID。
| redirect_uri  | 必需    | 要向其发送响应供应用处理的重定向 URI。它必须完全匹配在门户中注册的重定向 URI 之一，但它必须采用 URL 编码，且可以拥有其他路径段。
| state         | 建议 | 请求中包含的值，也会在令牌响应中返回。它可以是你希望的任何内容的字符串。此状态用于在发生身份验证请求前，对应用中的用户状态信息进行编码（例如它们所在的页面或视图上）。

### <a name="administrator-consent-experience"></a>管理员同意体验

对于 `/adminconsent` 终结点的请求，Azure AD 强制规定，仅租户管理员可以登录来完成请求。系统可能会提示管理员批准你在应用注册门户中为应用请求获取的所有应用程序权限。

下面的示例展示了 Azure AD 向管理员显示的同意对话框：

![管理员同意对话框。](./images/admin-consent.png)

### <a name="response"></a>响应

如果管理员批准应用程序的权限，则成功响应如下所示：

```
// Line breaks are for legibility only.

GET https://localhost/myapp/permissions
?tenant=a8990e1f-ff32-408a-9f8e-78d3b9139b95&state=12345
&admin_consent=True
```

| 参数     | 说明
|:--------------|:------------
| 租户        | 以 GUID 格式向应用程序授予其请求的权限的目录租户。
| state         | 请求中包含的值，也会在令牌响应中返回。它可以是你希望的任何内容的字符串。此状态用于在发生身份验证请求前，对应用中的用户状态信息进行编码（例如它们所在的页面或视图上）。
| admin_consent | 设置为 **true**。


> **试一试**：可以通过将下面的请求粘贴到浏览器中自行尝试。如果以 Azure AD 租户的全局管理员身份登录，你将看到应用的管理员同意对话框。（这与上文的同意对话框屏幕截图中显示的应用不同。）
> 
> https://login.microsoftonline.com/common/adminconsent?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&state=12345&redirect_uri=https://localhost/myapp/permissions 

## <a name="4-get-an-access-token"></a>4. 获取访问令牌

在 OAuth 2.0 客户端凭据授予流中，可使用在注册应用时保存的应用程序 ID 和应用程序密码值直接从 Microsoft 标识平台 `/token` 终结点请求访问令牌。

你可以通过传递 `https://graph.microsoft.com/.default` 并将其作为令牌请求中 `scope` 参数的值来指定预配置的权限。请参阅下面的令牌请求中的 `scope` 参数说明获取详情。

### <a name="token-request"></a>令牌请求

可将 POST 请求发送到 `/token` 标识平台终结点来获取访问令牌：

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

| 参数     | 条件 | 说明 
|:--------------|:----------|:------------
| 租户        | 必需  | 需要从中请求权限的目录租户。它可以 GUID 或友好名称格式显示。
| client_id     | 必需  | 注册应用时由 [Azure 应用注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)分配的应用程序 ID。
| 范围         | 必需  | 为此请求中的 `scope` 参数传递的值应为所需资源的资源标识符（应用程序 ID URI），带有 `.default` 后缀。 对于 Microsoft Graph，值为 `https://graph.microsoft.com/.default`。 此值会通知 Microsoft 标识平台终结点你在应用注册门户为应用配置的所有应用程序权限，它应该为与你要使用的资源关联的应用颁发令牌。
| client_secret | 必需  | 在应用注册门户中为应用生成的应用程序密码。请确保它已进行 URL 编码。
| grant_type    | 必需  | 必须是 `client_credentials`。

#### <a name="token-response"></a>令牌响应

成功的响应如下所示：

```json
{
  "token_type": "Bearer",
  "expires_in": 3599,
  "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik1uQ19WWmNBVGZNNXBP..."
}
```

| 参数     | 说明
|:--------------|:------------
| access_token  | 请求的访问令牌。应用可使用此令牌调用 Microsoft Graph。
| token_type    | 表示令牌类型值。Azure AD 唯一支持的类型是 `bearer`
| expires_in    | 访问令牌的有效期是多久（以秒为单位）。

## <a name="5-use-the-access-token-to-call-microsoft-graph"></a>5.使用访问令牌调用 Microsoft Graph

拥有访问令牌之后，可以通过将其包含在请求的 `Authorization` 标头中，用其调用 Microsoft Graph。以下请求可以获取特定用户的个人资料。你的应用必须拥有 _User.Read.All_ 权限才能调用此 API。

```
GET https://graph.microsoft.com/v1.0/users/12345678-73a6-4952-a53a-e9916737ff7f
Authorization: Bearer eyJ0eXAiO ... 0X2tnSQLEANnSPHY0gKcgw
Host: graph.microsoft.com
```
成功的响应将与此类似（一些响应标头已被删除）：

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

## <a name="supported-app-scenarios-and-resources"></a>受支持的应用场景和资源

以它们自己的标识调用 Microsoft Graph 的应用可分为两个类别：

- 在服务器上运行的没有登录用户的[后台服务（守护程序）](/azure/active-directory/develop/scenario-daemon-overview)。
- 具有登录用户但仍以它们自己的标识调用 Microsoft Graph 的应用；例如，使用需要具有比登录用户所拥有的提升权限更多权限的功能。

使用它们自己的标识调用 Microsoft Graph 的应用使用 OAuth 2.0 客户端凭据授予流通过 Azure AD 进行身份验证并获取访问令牌。对于 Microsoft 标识平台端点，可以使用以下资源进一步了解此方案:

- 有关还包含错误响应的客户端凭据授予流的更完整的处理，请参阅 [Azure Active Directory v2.0 和 OAuth 2.0 客户端凭据流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)。
- 有关从服务中调用 Microsoft Graph 的示例，请参阅 GitHub 上的 [v2.0 守护程序示例](https://github.com/Azure-Samples/active-directory-dotnet-daemon-v2)。
- 要详细了解所推荐的 Microsoft 和第三方身份验证库，请参阅 [ 标识平台身份验证库](/azure/active-directory/develop/reference-v2-libraries)。

## <a name="endpoint-considerations"></a>终结点注意事项

Microsoft 继续支持 Azure AD 终结点。 在使用 Microsoft 标识平台终结点和使用 Azure AD 终结点之间存在[诸多区别](/azure/active-directory/develop/azure-ad-endpoint-comparison)。 使用 Azure AD 终结点时：

- 如果你的应用是多租户的，则必须在 [Azure 门户](https://portal.azure.com)中将其明确配置为“多租户”。
- 没有管理员同意终结点 (`/adminconsent`)。但是，应用可以在运行时通过将 `prompt=admin_consent` 参数添加到授权请求来请求管理员同意。有关详细信息，请参阅 **在运行时触发 Azure AD 同意框架** 在 [ 将应用程序与 Azure Active Directory 集成](/azure/active-directory/develop/active-directory-integrating-applications)。
- 授权和令牌请求中的参数不相同。例如，Azure AD 终结点请求中没有 `scope` 参数；但是，`resource` 参数可用于指定为其请求的授权（用于管理员同意）或令牌的资源 (`resource=https://graph.microsoft.com`) 的 URI。

可查看下述资源进一步了解此方案：

- 要了解如何将 Microsoft 标识平台与不同类型的应用结合使用，请参阅 [Microsoft 标识平台文档](/azure/active-directory/develop/active-directory-developers-guide)中的 **开始使用** 链接。 该指南包含众多链接，可通过它们查看 Microsoft 标识平台支持的不同类型的应用的概述主题、快速入门、教程、代码示例和协议文档。
- 要了解可与 Microsoft 标识平台终结点结合使用的 Microsoft 身份验证库 (MSAL) 和服务器中间件，请参阅 [Microsoft 身份验证库](/azure/active-directory/develop/active-directory-authentication-libraries)。


## <a name="see-also"></a>另请参阅

- 有关 Azure 应用服务上托管的 Web 应用调用 Microsoft Graph 作为应用程序（使用托管标识）的示例，请参阅[教程：从安全应用访问作为应用的 Microsoft Graph](/azure/app-service/scenario-secure-app-access-microsoft-graph-as-app)。 本教程介绍如何在 web 应用上创建系统分配的托管标识、向托管标识添加 Microsoft Graph API 权限以及调用 Microsoft Graph。
- 有关使用 Microsoft 标识平台保护不同应用程序类型的示例，请查看 [Microsoft 标识平台代码示例 (v2.0 终结点)](/azure/active-directory/develop/sample-v2-code)。
