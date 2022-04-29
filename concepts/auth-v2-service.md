---
title: 在没有用户的情况下获取访问权限
description: 一些应用使用他们自己的标识（而不代表用户）调用 Microsoft Graph。 在许多情况下，这些应用是在服务器上运行且不存在已登录用户的后台服务或守护程序。
author: jackson-woods
ms.localizationpriority: high
ms.prod: applications
ms.custom: graphiamtop20
ms.openlocfilehash: 1fd849f0176468c76353f9f2c478dfca0b753027
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133424"
---
# <a name="get-access-without-a-user"></a>无用户访问

一些应用使用他们自己的标识（而不是代表用户）调用 Microsoft Graph。在许多情况下，这些是在服务器上运行且不存在已登录用户的后台服务或守护程序。此类应用的一个示例是在夜间唤醒并运行的电子邮件存档服务。在某些情况下，具有登录用户的应用也可能需要使用自己的标识调用 Microsoft Graph。例如，应用可能需要使用要求在组织中具有比登录用户更多的提升权限的功能。  

通过自己的标识调用 Microsoft Graph 的应用使用 OAuth 2.0 [客户端凭据授予流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 从 Azure AD 获取访问令牌。本文介绍了配置服务和使用 OAuth 客户端凭据授予流获取访问令牌的基本步骤。

## <a name="authentication-and-authorization-steps"></a>身份验证和授权步骤

请按照下列基本步骤来配置服务并从 Microsoft 标识平台终结点获取令牌。你的服务可以使用该令牌在其自身标识下调用 Microsoft Graph。

1. 注册应用。
2. 在应用上配置 Microsoft Graph 的权限。
3. 获取管理员同意。
4. 获取访问令牌。
5. 使用访问令牌调用 Microsoft Graph。

## <a name="1-register-your-app"></a>1.注册你的应用程序

要向 Microsoft 标识平台终结点进行身份验证，必须先在 [Azure 应用注册门户](https://go.microsoft.com/fwlink/?linkid=2083908)注册你的应用。你可使用 Microsoft 帐户或工作/学校帐户来注册应用。

对于将以自己的标识调用 Microsoft Graph 的服务，用户需要将应用注册到 Web 平台并复制以下值：

- Azure 应用注册门户分配的应用程序 ID。
- 客户端（应用程序）机密，可以是一个密码或是一个公钥/私钥对（证书）。
- 服务用于接收令牌响应的重定向 URL。
- 在应用实现请求管理员同意的功能时，服务用于接收管理员同意答复的重定向 URL。  

要分步了解如何通过 Azure 应用注册门户配置应用，请参阅[注册应用](./auth-register-app-v2.md)。

借助 OAuth 2.0 客户端凭据授予流，应用可使用 Azure AD 分配的应用程序 ID 以及通过门户创建的客户端机密在 Microsoft 标识平台 `/token` 终结点处直接进行身份验证。

## <a name="2-configure-permissions-for-microsoft-graph"></a>2.配置 Microsoft Graph 的权限

Microsoft Graph 为以自己的标识调用 Microsoft Graph 的应用公开 **应用程序权限**（Microsoft Graph 还为代表用户调用 Microsoft Graph 的应用公开委派权限）。

在注册应用时，应当预配置应用需要的应用程序权限。应用程序权限始终需要管理员的同意。当你的应用安装在他们的组织中时，管理员可以使用 [Azure 门户](https://portal.azure.com) 同意这些权限。你也可以在应用中提供注册体验，以便管理员通过此体验同意你配置的权限。Azure AD 记录管理员同意后，你的应用无需再次请求同意即可请求令牌。有关通过 Microsoft Graph 提供的权限的更多详细信息，请参阅 [权限参考](./permissions-reference.md)

要在 [Azure 应用注册门户](https://go.microsoft.com/fwlink/?linkid=2083908) 为应用配置应用程序权限，请在应用程序的“**API 权限**”页面下，依次选择“**添加权限**”和“**Microsoft Graph**”，然后在“**应用程序权限**”下选择应用所需的权限。

下面的屏幕快照显示了 Microsoft Graph 应用程序权限的“**选择权限**”对话框。

:::image type="content" source="./images/auth-v2/v2-application-permissions.png" alt-text="Microsoft Graph 应用程序权限的“选择权限”窗口。" border="true":::

> [!IMPORTANT]
> 
> 配置应用所需的一组最低特权权限，以提高其安全性。 有关详细信息，请参阅 [使用最低特权原则增强安全性](/azure/active-directory/develop/secure-least-privileged-access)。

## <a name="3-get-administrator-consent"></a>3.获取管理员同意

你可让管理员在 [Azure 门户](https://portal.azure.com)授予你的应用所需的权限；但通常情况下，更好的方法是通过 Microsoft 标识平台 `/adminconsent` 终结点提供管理员注册体验。 

> [!IMPORTANT]
> 
> 更改已配置的权限时，还必须重复执行该管理员同意过程。 租户管理员重新应用同意之后，才会反映应用注册门户中所做的更改。

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
| 租户        | 必需    | 希望从中请求权限的目录租户。值可以采用 GUID 或易记名称格式。如果不了解用户属于哪个租户，并且希望用户使用任意租户登录，请使用 `common`。
| client_id     | 必需    | [Azure 应用注册门户](https://go.microsoft.com/fwlink/?linkid=2083908) 分配给你的应用的应用程序 ID。
| redirect_uri  | 必需    | 要向其发送答复以供应用处理的重定向 URI。必须与你在门户中注册的重定向 URI 之一相匹配。必须采用 URL 编码，并且可以具有其他路径段。
| state         | 建议 | 请求中包含的值，也会在令牌响应中返回。它可以是你希望的任何内容的字符串。此状态用于在发生身份验证请求前，对应用中的用户状态信息进行编码（例如它们所在的页面或视图上）。

### <a name="administrator-consent-experience"></a>管理员同意体验

对于向 `/adminconsent` 终结点的请求，Azure AD 强制要求仅租户管理员可以登录来完成请求。系统可能要求管理员批准你已在应用注册门户中为应用请求的所有应用程序权限。

下面的屏幕截图是 Azure AD 向管理员显示的同意对话框示例：

:::image type="content" source="./images/auth-v2/admin-consent.png" alt-text="管理员同意对话框。" border="true":::

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


> **试一试**：可以通过将下面的请求粘贴到浏览器中自行尝试此设置。如果以 Azure AD 租户的全局管理员身份登录，你将看到应用的管理员同意对话框。（此应用与上文显示的同意对话框屏幕截图中的应用不同。）
> 
> https://login.microsoftonline.com/common/adminconsent?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&state=12345&redirect_uri=https://localhost/myapp/permissions 

## <a name="4-get-an-access-token"></a>4. 获取访问令牌

在 OAuth 2.0 客户端凭据授予流中，可使用在注册应用时保存的应用程序 ID 和客户端密码值直接从 Microsoft 标识平台 `/token` 终结点请求访问令牌。

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
| 租户        | 必需  | 希望从中请求权限的目录租户。值可以采用 GUID 或易记名称格式。
| client_id     | 必需  | 注册应用时由 [Azure 应用注册门户](https://go.microsoft.com/fwlink/?linkid=2083908) 分配的应用程序 ID。
| 范围         | 必需  | 为此请求中的 **scope** 参数传递的值应为所需资源的标识符（应用程序 ID URI），带有 `.default` 后缀。 例如，Microsoft Graph 资源应用 ID URI 为 `https://graph.microsoft.com/`。 因此，对于 Microsoft Graph，**scope** 的值为 `https://graph.microsoft.com/.default`。 此值通知 Microsoft 标识平台终结点将管理员同意的所有应用级别权限包含在访问令牌中。
| client_secret | 必需  | 在应用注册门户中为应用生成的客户端密码。请确保它已进行 URL 编码。
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
成功的响应外观将与此类似（一些响应标头已被删除）：

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
- 具有登录用户但仍以其自己的标识调用 Microsoft Graph 的应用；例如，要使用需要比该用户更多的提升权限的功能。

使用它们自己的标识调用 Microsoft Graph 的应用使用 OAuth 2.0 客户端凭据授予流通过 Azure AD 进行身份验证并获取访问令牌。对于 Microsoft 标识平台端点，可以使用以下资源进一步了解此方案:

- 有关还包含错误响应的客户端凭据授予流的更完整的处理，请参阅 [Azure Active Directory v2.0 和 OAuth 2.0 客户端凭据流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)。
- 有关从服务中调用 Microsoft Graph 的示例，请参阅 GitHub 上的 [v2.0 守护程序示例](https://github.com/Azure-Samples/active-directory-dotnet-daemon-v2)。
- 要详细了解所推荐的 Microsoft 和第三方身份验证库，请参阅 [ 标识平台身份验证库](/azure/active-directory/develop/reference-v2-libraries)。

## <a name="endpoint-considerations"></a>终结点注意事项

Microsoft 继续支持 Azure AD 终结点。 在使用 Microsoft 标识平台终结点和使用 Azure AD 终结点之间存在[诸多区别](/azure/active-directory/develop/azure-ad-endpoint-comparison)。 使用 Azure AD 终结点时：

- 如果你的应用是多租户的，则必须在 [Azure 门户](https://portal.azure.com)中将其明确配置为“多租户”。
- 不存在管理员同意终结点 ()，但是，你的应用可以在运行时期间通过将 `prompt=admin_consent` 参数添加到授权请求来请求管理员同意。要了解详细信息，请参阅 [将应用程序与 Azure Active Directory 相集成](/azure/active-directory/develop/active-directory-integrating-applications) 中的 **在运行时引发 Azure AD 同意框架**。
- 授权和令牌请求中的参数不相同。例如，Azure AD 终结点请求中不存在 `scope` 参数；但使用 `resource` 参数来指定为其请求的授权（用于管理员同意）或令牌的资源（`resource=https://graph.microsoft.com`）的 URI。

可查看下述资源进一步了解此方案：

- 要了解如何将 Microsoft 标识平台与不同类型的应用结合使用，请参阅 [Microsoft 标识平台文档](/azure/active-directory/develop/active-directory-developers-guide)中的 **开始使用** 链接。
- 要了解可与 Microsoft 标识平台终结点结合使用的 Microsoft 身份验证库 (MSAL) 和服务器中间件，请参阅 [Microsoft 身份验证库](/azure/active-directory/develop/active-directory-authentication-libraries)。


## <a name="see-also"></a>另请参阅

- [根据方案选择 Microsoft Graph 身份验证提供程序](/graph/sdks/choose-authentication-providers?tabs=CS)
- [了解如何创建在其自己的标识下调用 Microsoft Graph 的 Web 应用](/azure/app-service/scenario-secure-app-access-microsoft-graph-as-app)。
- 有关使用 Microsoft 标识平台保护不同应用程序类型的示例，请参阅 [Microsoft 标识平台代码示例（v2.0 终结点）](/azure/active-directory/develop/sample-v2-code)。
