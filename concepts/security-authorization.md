---
title: 授权和 Microsoft Graph 安全性 API
description: 可通过 Microsoft Graph 安全性 API 访问的安全数据是很敏感的，它受到权限和 Azure Active Directory (Azure AD) 角色保护。
ms.openlocfilehash: c69621fa7059a96381bed76b58c4a77e80d984dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091741"
---
# <a name="authorization-and-the-microsoft-graph-security-api"></a>授权和 Microsoft Graph 安全性 API

可通过 Microsoft Graph 安全性 API 访问的安全数据是很敏感的，它受到权限和 Azure Active Directory (Azure AD) 角色保护。

Microsoft Graph 安全性 API 支持以下两种类型的授权：

- **应用级授权** - 没有已登录用户（例如，SIEM 方案）。 授权由授予给应用程序的权限决定。 
    >**注意：** 此选项还可以支持基于角色的访问控制 (RBAC) 由应用程序管理的情况。
- **用户委派授权** - 身份为 Azure AD 租户成员的用户已登录。 除了已被授予所需权限的应用程序之外，用户必须是 Azure AD 有限管理员角色的成员 - 安全读者或安全管理员。

若要从 Graph 浏览器调用 Microsoft Graph 安全性 API：

- Azure AD 租户管理员必须对 Graph 浏览器应用显式授予所请求的权限。
- 用户必须是 Azure AD 中安全读者有限管理员角色的成员（安全读者或安全管理员）。

>**注意**：Graph 浏览器不支持应用级授权。

若要从自定义应用或你自己的应用调用 Microsoft Graph 安全性 API：

- Azure AD 租户管理员必须对你的应用显式授权。 这对于应用程序级别授权和用户委派授权都是必需的。
- 如果正在使用用户委派授权，用户必须是 Azure AD 中安全读者或安全管理员有限管理员角色的成员。

## <a name="manage-authorization-in-security-api-client-applications"></a>管理安全性 API 客户端应用中的授权

通过 Microsoft Graph 安全性 API 提供的安全数据是很敏感的，必须受到适当身份验证和授权机制的保护。 下表列出了注册和创建可访问 Microsoft Graph 安全性 API 的客户端应用的步骤。

| **谁** | **操作** |
|:---------------------|:------------------|
|应用程序开发人员或所有者：|将应用程序注册为企业应用程序。|
|租户管理员|向应用程序授予权限。|
|租户管理员|为用户分配角色。|
|应用开发人员|以用户身份登录，并使用应用访问 Microsoft Graph 安全性 API。|

应用注册仅定义运行应用所需的权限。 它不对应用程序进行这些权限的授予。

Azure AD 租户管理员必须对应用程序显式授予权限。 这必须按每租户实施，并且必须在应用程序权限在应用程序注册门户中*每次更改时执行*。

例如，假定你拥有一个应用程序、两个 Azure AD 租户（**T1** 和 **T2**），以及两个权限（**P1** 和 **P2**）。 以下是授权过程：

- 应用程序注册以请求权限 **P1**。
- 当租户 **T1** 中的用户获取此应用程序的 Azure AD 令牌时，该令牌不包含任何权限。
- 租户 **T1** 的 Azure AD 管理员向应用程序显式授予权限。 当租户 **T1** 中的用户获取应用程序的 Azure AD 令牌时，它将包含权限 **P1**。
- 当租户 **T2** 中的用户获取应用程序的 Azure AD 令牌时，该令牌不包含任何权限，因为租户 **T2** 的管理员尚未向该应用程序授予权限。 权限必须按照*每个租户*和*每个应用程序*进行授予。
- 应用程序将其注册更改为现在需要权限 **P1** 和 **P2**。
- 当租户 **T1** 中的用户获取应用程序的 Azure AD 令牌时，它仅包含权限 **P1**。 授予应用程序的权限作为授予内容快照进行记录，它们在应用程序注册（权限）更改后*不会自动更改*。
- 租户 **T2** 的管理员对应用程序授予权限 **P1** 和 **P2**。 当租户 **T2** 中的用户获取应用程序的 Azure AD 令牌时，该令牌将包含权限 **P1** 和 **P2**。

>**注意**：租户 **T1** 中的应用程序和租户 **T2** 中的应用程序的 Azure AD 令牌包含不同权限，因为每个租户管理员已为应用程序授予不同的权限。

- 如需使租户 **T1** 中的应用程序再次运行，租户 **T1** 的管理员必须向应用程序显式授予权限 **P1** 和 **P2**。

## <a name="register-an-application-in-the-azure-ad-v20-endpoint"></a>在 Azure AD v2.0 终结点中注册应用程序

如需将应用程序注册到 Azure AD v2.0 终结点，将需要：

- **应用程序名称** - 表示应用程序名称的字符串。
- **重定向 URL** - 该 URL 发送来自 Azure AD 的身份验证响应。 请使用测试客户端 web 应用主页以开始。
- **所需的权限** - 应用程序需要的用于调用 Microsoft Graph 的权限。

注册应用程序：

1. 转到 https://apps.dev.microsoft.com/ 并登录。
    >**注意**：你无需是租户管理员。你将被重定向到“**我的应用程序**”列表。
2. 选择“**添加应用**”，并输入“**应用程序名称**”以创建新应用程序。
3. 在新应用程序注册页面，选择“**添加平台**” > “**Web**”。 在“**重定向 URL**”字段中，输入重定向 URL。
4. 在“**Microsoft Graph 权限**”部分的“**委派权限**”下，选择“**添加**”。 在对话框中，选择所需的权限。 如需查看权限列表，请参阅[安全权限](permissions-reference.md#security-permissions)。

    >Microsoft Graph 安全性 API 要求，必须对 GET 查询使用 SecurityEvents.Read.All 作用域，并对 PATCH/POST 查询使用 SecurityEvents.ReadWrite.All 作用域。

5. 选择“保存”****。

保存以下信息：

- 应用程序 ID
- 重定向 URL
- 所需权限列表

如需了解更多信息，请参阅[使用 Azure AD v2.0 终结点注册应用](auth-register-app-v2.md)。

## <a name="grant-permissions-to-an-application"></a>向应用程序授予权限

应用程序注册仅定义应用程序所需的权限，它并不向应用程序授予这些权限。 Azure AD 租户管理员必须通过调用管理员许可终结点来显示授予这些权限。 如需了解详细信息，请参阅[使用管理员许可终结点](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/active-directory-v2-scopes#using-the-admin-consent-endpoint)。

如要向应用程序授予权限，将需要：

- **应用程序 ID** - 应用程序注册门户中的应用程序 ID。
- **重定向 URL** - 在应用程序注册门户中为身份验证响应设置的字符串。

如要授予权限，请执行下列操作：

- 在文本编辑器中创建以下 URL 字符串：

    `https://login.microsoftonline.com/common/adminconsent?client_id=<Application Id>&state=12345&redirect_uri=<Redirect URL>`

- 在 web 浏览器中转到此 URL，并以租户管理员身份登录。 对话框将显示应用程序需要的权限列表，如应用程序注册门户中所指定的。 选择“**确定**”，以向应用程序授予这些权限。

> **注意：** 此步骤向应用程序授予权限，而不是向用户授权。 这意味着属于 Azure AD 租户的所有使用此应用程序的用户将被授予权限，甚至包括非管理员用户。

## <a name="assign-azure-ad-roles-to-users"></a>向用户分配 Azure AD 角色

应用程序被授予权限后，每个可以访问该应用程序的人（即 Azure AD 租户的成员）都将获得已授予的权限。 为了进一步保护敏感安全数据，Microsoft Graph 安全性 API 还要求必须为用户分配 Azure AD **安全读者**角色。 有关详细信息，请参阅[分配管理员角色](https://docs.microsoft.com/zh-CN/azure/active-directory/active-directory-assign-admin-roles-azure-portal)和[为用户分配管理员角色](https://docs.microsoft.com/zh-CN/azure/active-directory/active-directory-users-assign-role-azure-portal)。

>**注意：** 必须是租户管理员才能执行此步骤。

若要为用户分配角色：

- 登录到 [Azure 门户](https://portal.azure.com) (https://portal.azure.com)。
- 在菜单中，选择“**Azure Active Directory**” > “**用户**”。
- 选择用户名称。
- 选择“**管理**” > “**目录角色**”。
- 选择“**有限管理员**”，然后选中“**安全读者**”复选框。
- 选择“**保存**”。

## <a name="create-an-authentication-code"></a>创建身份验证代码

若要创建身份验证代码，将需要：

- **应用程序 ID** - 应用程序注册门户中的应用程序 ID。
- **重定向 URL** - 该 URL 发送来自 Azure AD 的身份验证响应。 请使用 https://localhost 或测试客户端 web 应用主页以开始。
- **应用程序密钥**（可选）- 应用程序的密钥。 这适用于将使用仅应用程序身份验证代码（即不支持用户委派身份验证）的应用程序的开发。

下表列出了可用于创建身份验证代码的资源。

|**应用程序类型**|**身份验证库**|
|------------------------|----------------------------|
|[桌面应用 - iOS](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/guidedsetups/active-directory-ios)|[MSAL.framework：适用于 iOS 的 Microsoft 身份验证库预览版](https://github.com/AzureAD/microsoft-authentication-library-for-objc)|
|[桌面应用 - Android](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/guidedsetups/active-directory-android)|[Microsoft 身份验证库 (MSAL)](https://javadoc.io/doc/com.microsoft.identity.client/msal)|
|[桌面应用 - .Net](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/guidedsetups/active-directory-windesktop)|[Microsoft 身份验证库 (MSAL)](https://www.nuget.org/packages/Microsoft.Identity.Client)|
|[Web 应用 - JavaScript SPA](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/guidedsetups/active-directory-javascriptspa)|[适用于 JavaScript 的 Microsoft 身份验证库预览版](https://github.com/AzureAD/microsoft-authentication-library-for-js)|
|[Web 应用 - .NET Web 服务器](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/guidedsetups/active-directory-aspnetwebapp)|OpenIdConnection、Cookie、SystemWeb|
|[Web 应用 - NodeJS Web 应用](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/active-directory-v2-devquickstarts-node-web)||

对于不使用任何现有库的应用程序，请参阅[代表用户获取访问权限](auth-v2-user.md)。

1. 从 Azure AD 获取代码。 调用的查询包含应用程序 ID 参数、重定向 URl 和**所需的权限**。
2. 使用代码获取访问令牌。

如果你使用 OpenId Connect 库，请参阅[使用 Azure AD 和 OpenID Connect 进行身份验证](https://docs.microsoft.com/zh-CN/azure/architecture/multitenant-identity/authenticate)并调用 `app.UseOpenIdConnectAuthentication()`。

>**注意：** 如果请求的是用户委派身份验证令牌，库的参数是**请求的作用域**。 请对该参数使用 User.Read，而非注册的应用程序所要求的值。 **请求的作用域**参数不影响包含在返回身份验证令牌中的权限。 这些由租户管理员授予应用程序的权限所确定。

例如，如果使用 .NET MSAL 库，请执行以下调用：

`var accessToken = (await client.AcquireTokenAsync(scopes)).AccessToken;`

>**注意：** 此示例应使用最低的许可权限，如 User.Read。 但是，返回的访问令牌可包含由租户管理员授予当前用户租户的权限，如 User.Read.All 或 User.ReadWrite.All。

Azure AD 返回的令牌（字符串）包含身份验证信息和应用程序所需的权限。 将此令牌作为持有者令牌分配到 HTTP 标头，如下例所示。

`request.Headers.Authorization = new AuthenticationHeaderValue("bearer", accessToken);`

Microsoft Graph 将验证包含在此令牌中的信息，并授予或拒绝访问权限。

如要查看包含在返回令牌中的声明，请使用 NuGet 库 System.IdentityModel.Tokens.Jwt。

`JwtSecurityTokenHandler tokenHandler = new JwtSecurityTokenHandler();`</br>
`var securityToken = tokenHandler.ReadToken(accessToken) as JwtSecurityToken;`

来自 Microsoft Graph 的响应包含一个被称为 client-request-id 的标头，这是一个 GUID。 如果访问被拒绝，在 [Microsoft 技术社区](https://techcommunity.microsoft.com/t5/Microsoft-Graph-Security-API/ct-p/SecurityGraphAPI)寻求支持时请指明此 GUID，以便帮助调查此身份验证故障的原因。
