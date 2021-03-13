---
title: Microsoft Graph 身份验证和授权基础知识
description: 要调用 Microsoft Graph，应用必须从 Microsoft 标识平台获取一个访问令牌。
author: matt-steele
localization_priority: Priority
ms.prod: applications
ms.custom: graphiamtop20
ms.openlocfilehash: 731518e03441562424a09e86a57f61091cdc9cf8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760726"
---
# <a name="authentication-and-authorization-basics-for-microsoft-graph"></a>Microsoft Graph 身份验证和授权基础知识

要调用 Microsoft Graph，应用必须从 Microsoft 标识平台获取一个访问令牌。 访问令牌包含你的应用的相关信息，还有它就可通过 Microsoft Graph 访问的资源和 API 所具备的权限。 要获取访问令牌，你的应用必须向 Microsoft 标识平台注册，并获得用户或管理员的授权可访问其所需的 Microsoft Graph 资源。

本主题简要概述了访问令牌、Microsoft 标识平台，以及应用可获取访问令牌的方式。 如果你已熟悉如何将应用与 Microsoft 标识平台集成来获取令牌，请参阅[后续步骤](#next-steps)部分，以了解相关信息并查看 Microsoft Graph 特定的示例。

## <a name="access-tokens"></a>访问令牌

Microsoft 标识平台发布的访问令牌包含受 Microsoft 标识平台保护的 Web API （如 Microsoft Graph，用于验证调用方和确保调用方具有适当的权限来执行其请求的操作）的信息（声明）。 调用 Microsoft Graph 时，应将访问令牌视为不透明。 必须始终通过传输层安全性 (HTTPS) 等安全通道来传输访问令牌。

下面是一个 Microsoft 标识平台访问令牌示例：

```jwt
EwAoA8l6BAAU7p9QDpi/D7xJLwsTgCg3TskyTaQAAXu71AU9f4aS4rOK5xoO/SU5HZKSXtCsDe0Pj7uSc5Ug008qTI+a9M1tBeKoTs7tHzhJNSKgk7pm5e8d3oGWXX5shyOG3cKSqgfwuNDnmmPDNDivwmi9kmKqWIC9OQRf8InpYXH7NdUYNwN+jljffvNTewdZz42VPrvqoMH7hSxiG7A1h8leOv4F3Ek/oeJX6U8nnL9nJ5pHLVuPWD0aNnTPTJD8Y4oQTp5zLhDIIfaJCaGcQperULVF7K6yX8MhHxIBwek418rKIp11om0SWBXOYSGOM0rNNN59qNiKwLNK+MPUf7ObcRBN5I5vg8jB7IMoz66jrNmT2uiWCyI8MmYDZgAACPoaZ9REyqke+AE1/x1ZX0w7OamUexKF8YGZiw+cDpT/BP1GsONnwI4a8M7HsBtDgZPRd6/Hfqlq3HE2xLuhYX8bAc1MUr0gP9KuH6HDQNlIV4KaRZWxyRo1wmKHOF5G5wTHrtxg8tnXylMc1PKOtaXIU4JJZ1l4x/7FwhPmg9M86PBPWr5zwUj2CVXC7wWlL/6M89Mlh8yXESMO3AIuAmEMKjqauPrgi9hAdI2oqnLZWCRL9gcHBida1y0DTXQhcwMv1ORrk65VFHtVgYAegrxu3NDoJiDyVaPZxDwTYRGjPII3va8GALAMVy5xou2ikzRvJjW7Gm3XoaqJCTCExN4m5i/Dqc81Gr4uT7OaeypYTUjnwCh7aMhsOTDJehefzjXhlkn//2eik+NivKx/BTJBEdT6MR97Wh/ns/VcK7QTmbjwbU2cwLngT7Ylq+uzhx54R9JMaSLhnw+/nIrcVkG77Hi3neShKeZmnl5DC9PuwIbtNvVge3Q+V0ws2zsL3z7ndz4tTMYFdvR/XbrnbEErTDLWrV6Lc3JHQMs0bYUyTBg5dThwCiuZ1evaT6BlMMLuSCVxdBGzXTBcvGwihFzZbyNoX+52DS5x+RbIEvd6KWOpQ6Ni+1GAawHDdNUiQTQFXRxLSHfc9fh7hE4qcD7PqHGsykYj7A0XqHCjbKKgWSkcAg==
```

要调用 Microsoft Graph，请将访问令牌作为 持有者令牌附加到 HTTP 请求的授权标头中。 例如，下述调用会返回已登录用户的个人资料信息（已缩短访问令牌以便于阅读）：

```http
GET https://graph.microsoft.com/v1.0/me/ HTTP/1.1
Host: graph.microsoft.com
Authorization: Bearer EwAoA8l6BAAU ... 7PqHGsykYj7A0XqHCjbKKgWSkcAg==
```

## <a name="register-your-app-with-the-microsoft-identity-platform"></a>向 Microsoft 标识平台注册应用

必须在 [Azure 门户](https://portal.azure.com/)中注册应用，然后它才能从 Microsoft 标识平台获取令牌。 注册会将应用与 Microsoft 标识平台相集成，并建立用于获取令牌的信息，其中包括：

- **应用程序 ID**：Microsoft 标识平台分配的唯一标识符。
- **重定向 URI/URL**：应用从 Microsoft 标识平台接收响应时要用到的一个或多个终结点。 （对于本机和移动应用，它是 Microsoft 标识平台分配的 URI。）
- **应用程序密码**： 密码或您的应用程序使用进行 Microsoft 的标识平台身份验证一个公共/私钥对。 （不是本机或移动应用的必需项。）

请求中会使用在注册期间配置的属性。 例如，在以下令牌请求中：*client_id* 是 *应用程序 ID*，*redirect_uri* 是应用注册的某个 *重定向 URL*，*client_secret* 则是 *应用程序密码*。

```http
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

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

Microsoft Graph 公开了控制应用程序对资源（如用户、组和邮件）的访问权限的粒度权限。 由开发者决定为 Microsoft Graph 请求哪些权限。 当用户登录你的应用时，他们或（某些情况下）管理员可同意这些权限。 如果用户同意，则你的应用可访问其请求的资源和 API。 对于没有用户登录的应用，在安装应用时，可由管理员预先同意权限。

### <a name="best-practices-for-requesting-permissions"></a>请求权限的最佳做法
[!INCLUDE [auth-use-least-privileged](../../includes/auth-use-least-privileged.md)]

### <a name="delegated-and-application-permissions"></a>委派权限和应用程序权限
Microsoft Graph 具有两种权限类型：

- **委派权限** 供已有用户登录的应用使用。 对于这些应用，用户或管理员同意应用请求的权限，并且应用可在调用 Microsoft Graph 时充当已登录的用户。 一些委派权限可由非管理用户同意，但一些特权级别更高的权限需要[管理员同意](/azure/active-directory/develop/active-directory-v2-scopes#using-the-admin-consent-endpoint)。  

- **应用程序权限** 由无需用户登录即可运行的应用使用；例如，作为后台服务或守护程序运行的应用。 应用程序权限只能[由管理员同意](/azure/active-directory/develop/active-directory-v2-scopes#requesting-consent-for-an-entire-tenant)。 

_有效权限_ 是应用在向 Microsoft Graph 发出请求时具有的权限。调用 Microsoft Graph 时，了解授予应用的委派权限及应用程序权限与其有效权限之间的区别非常重要。

- 对于委派权限，应用的有效权限将为已（通过同意）向应用授予的委派权限和当前登录用户的特权之间的交集。 应用具有的特权不得比已登录用户的多。 在组织内，已登录用户的特权可由策略或在一个或多个管理员角色中的成员资格确定。 若要详细了解管理员角色，请参阅[在 Azure Active Directory 中分配管理员角色](/azure/active-directory/active-directory-assign-admin-roles)。<br/><br/>例如，假定你的应用被授予 User.ReadWrite.All 委派权限。 此权限名义上授予应用读取和更新组织中每位用户个人资料的权限。 如果已登录的用户是全局管理员，则应用将能够更新组织中每个用户的配置文件。 但是，如果已登录的用户不具有管理员角色，则应用将只能更新已登录用户的配置文件。 它将无法更新组织中其他用户的个人资料，因为它有权代表执行操作的用户没有这些特权。
- 对于应用程序权限，应用的有效权限将与权限所暗示的特权完全相等。 例如，具有 User.ReadWrite.All 应用程序权限的应用可更新组织中每位用户的个人资料。

>**注意** 默认情况下，已将应用程序权限授予以下数据集的应用可访问组织中的所有邮箱：

- [日历](../permissions-reference.md#calendars-permissions)
- [联系人](../permissions-reference.md#contacts-permissions)
- [邮件](../permissions-reference.md#mail-permissions)
- [邮箱设置](../permissions-reference.md#mail-permissions)

>管理员可以配置 [应用程序访问策略](../auth-limit-mailbox-access.md)，以限制对 _特定_ 邮箱的应用访问。

要在完整列表中查看 Microsoft Graph 的委派权限和应用程序权限，以及哪些权限需要管理员同意，请参阅[权限参考](../permissions-reference.md)。

## <a name="getting-an-access-token"></a>获取访问令牌

与大多数开发人员一样，你可能会使用身份验证库来管理与 Microsoft 标识平台的令牌交互。 身份验证库从开发人员那里提取了许多协议细节，如验证、cookie 处理、令牌缓存和安全连接维持，让你能在应用上专注开发。 Microsoft 发布了开源客户端库和服务器中间件。

对于 Microsoft 标识平台终结点：

- Microsoft 身份验证库 (MSAL) 客户端库适用于 .NET、JavaScript、Android 和 Objective-c。所有平台都处于生产支持的预览下，而且，一旦引入重大更改，Microsoft 会保证升级的路径。
- 来自 Microsoft 的服务器中间件可用于 .NET core 和 ASP.NET（OWIN OpenID Connect 和 OAuth），还可用于 Node.js (Microsoft 标识平台 Passport.js)。
- Microsoft 标识平台与许多第三方身份验证库兼容。

要在完整列表中查看 Microsoft 客户端库、Microsoft 服务器中间件和兼容的第三方库，请参阅 [Microsoft 标识平台身份验证库](/azure/active-directory/develop/active-directory-v2-libraries)。

无需使用身份验证库即可获取访问令牌。 要了解如何在不使用身份验证库的情况下直接使用 Microsoft 标识平台终结点，请参阅 [Microsoft 标识平台身份验证](/azure/active-directory/develop/authentication-scenarios)

## <a name="next-steps"></a>后续步骤

- 有关如何为调用 Microsoft Graph 的应用获取访问令牌的快捷步骤，请选择与你的场景相符的应用类型：
  - [桌面应用](/azure/active-directory/develop/scenario-desktop-overview)
  - [移动应用](/azure/active-directory/develop/scenario-mobile-overview)
  - [Web 应用](/azure/active-directory/develop/scenario-web-app-call-api-overview)
  - [单页应用](/azure/active-directory/develop/scenario-spa-overview)
  - [守护程序/后台服务](/azure/active-directory/develop/scenario-daemon-overview)
- 若要查看你可以在 Microsoft Graph 中使用的权限，请参阅[权限](../permissions-reference.md)。
- 如果你是 Microsoft 云解决方案提供商并且对通过 Microsoft Graph 访问合作伙伴托管的客户数据感兴趣，请参阅[管理应用访问 (CSPs)](../auth-cloudsolutionprovider.md)。

如果已准备好跳到代码，可使用下述资源，它们可帮助你在应用中向 Microsoft 标识平台进行身份验证并获取授权。

### <a name="microsoft-graph-training-and-samples"></a>Microsoft Graph 培训和示例

为帮助你快速入门，我们创建了一系列的培训模块和其他资源，来向你展示如何在各类平台上进行身份验证和使用 API。

- 通过[使用入门](https://developer.microsoft.com/graph/get-started)页面查找你喜爱的平台所适用的库、示例、培训内容和其他资源。
- 要通过平台预配置的示例快速运行，请参阅 [Microsoft Graph 快速入门](https://developer.microsoft.com/graph/quick-start)。
- 请参阅 GitHub 上的 [Microsoft Graph 示例](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=sample&type=&language=)。

### <a name="microsoft-identity-platform-samples-and-documentation"></a>Microsoft 标识平台示例和文档

Microsoft 标识平台文档中有一些文章和示例，它们专门介绍如何向 Microsoft 标识平台进行身份验证以及如何获得它的授权。

- 要开始学习，最简单的是在 [Microsoft 标识平台终结点文档](/azure/active-directory/develop/active-directory-appmodel-v2-overview)。 本文中有概述链接、协议文档，还有入门文章来针对全部按你正在开发的应用类型整理的不同平台。
- 要了解客户端或服务器身份验证库列出的示例，请参阅 [Microsoft 标识平台身份验证库](/azure/active-directory/develop/active-directory-v2-libraries)。
- 在 [Azure 代码库](https://azure.microsoft.com/resources/samples/?service=active-directory)中按平台查看 Microsoft 标识平台示例。

## <a name="see-also"></a>另请参阅

- [Microsoft 标识平台终结点文档](/azure/active-directory/develop/active-directory-appmodel-v2-overview)