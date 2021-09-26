---
title: Microsoft Graph 身份验证和授权基础知识
description: 要调用 Microsoft Graph，应用必须从 Microsoft 标识平台获取一个访问令牌。
author: matt-steele
ms.localizationpriority: high
ms.prod: applications
ms.custom: graphiamtop20
ms.openlocfilehash: 877d3e2c1ce0d80ff625504bc2248d32d595f0ba
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507961"
---
# <a name="authentication-and-authorization-basics-for-microsoft-graph"></a>Microsoft Graph 身份验证和授权基础知识

为了调用 Microsoft Graph，应用必须从 Microsoft 标识平台获取访问令牌。该访问令牌包含应用相关信息以及它对可通过 Microsoft Graph 使用的资源和 API 所具有的权限。若要获取访问令牌，应用必须向 Microsoft 标识平台注册，并且获得用户或管理员的授权，可访问其所需的 Microsoft Graph 资源。

本文概述了访问令牌、Microsoft 标识平台，以及应用可获取访问令牌的方式。 如果你已知道如何将应用与 Microsoft 标识平台集成来获取令牌，请参阅 [后续步骤](#next-steps) 部分中的信息和特定于 Microsoft Graph 的示例。

## <a name="access-tokens"></a>访问令牌

Microsoft 标识平台发布的访问令牌包含以下信息（声明）：Web API 受到 Microsoft 标识平台（如 Microsoft Graph）的保护，用于验证调用方并确保调用方有相应的权限可执行其正在请求的操作。调用 Microsoft Graph 时，应将访问令牌视为不透明。始终可通过安全通道（例如传输层安全性 (HTTPS)）传输访问令牌。

下面是一个 Microsoft 标识平台访问令牌示例：

```jwt
EwAoA8l6BAAU7p9QDpi/D7xJLwsTgCg3TskyTaQAAXu71AU9f4aS4rOK5xoO/SU5HZKSXtCsDe0Pj7uSc5Ug008qTI+a9M1tBeKoTs7tHzhJNSKgk7pm5e8d3oGWXX5shyOG3cKSqgfwuNDnmmPDNDivwmi9kmKqWIC9OQRf8InpYXH7NdUYNwN+jljffvNTewdZz42VPrvqoMH7hSxiG7A1h8leOv4F3Ek/XbrnbEErTDLWrV6Lc3JHQMs0bYUyTBg5dThwCiuZ1evaT6BlMMLuSCVxdBGzXTBcvGwihFzZbyNoX+52DS5x+RbIEvd6KWOpQ6Ni+1GAawHDdNUiQTQFXRxLSHfc9fh7hE4qcD7PqHGsykYj7A0XqHCjbKKgWSkcAg==
```

若要调用 Microsoft Graph，请将访问令牌作为持有者令牌附加到 HTTP 请求中的授权标头。例如以下调用，它返回已登录用户的个人资料信息（为了可读性，已将访问令牌缩短）：

```http
GET https://graph.microsoft.com/v1.0/me/ HTTP/1.1
Host: graph.microsoft.com
Authorization: Bearer EwAoA8l6BAAU ... 7PqHGsykYj7A0XqHCjbKKgWSkcAg==
```

## <a name="register-your-app-with-the-microsoft-identity-platform"></a>向 Microsoft 标识平台注册应用

必须在 [Azure 门户](https://portal.azure.com/)中注册应用，然后它才能从 Microsoft 标识平台获取令牌。 注册会将应用与 Microsoft 标识平台相集成，并建立用于获取令牌的信息，其中包括：

- **应用程序 ID**：Microsoft 标识平台分配的唯一标识符。
- **重定向 URI/URL**: 应用将从 Microsoft 标识平台接收响应的一个或多个终结点。(对于本机和移动应用，此为 Microsoft 标识平台分配的 URI。)
- **应用程序密码**: 应用用于通过 Microsoft 标识平台进行身份验证的密码或公钥/私钥对。(本机或移动应用不需要。)

注册期间配置的属性应用于请求中。例如，在以下令牌请求中: *client_id* 为 *应用程序 ID*，*redirect_uri* 为应用的其中一个注册 *重定向 URI*，*client_secret* 为 *应用程密码*。

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

Microsoft Graph 公开可控制应用对资源（如用户、组和邮件）的访问的粒度权限。作为开发人员，你可决定为 Microsoft Grap 请求哪些权限。当用户登录你的应用时，他们（在某些情况下，可能是管理员）有机会同意这些权限。如果用户同意，则你的应用可访问其请求的资源和 API。对于没有已登录用户的应用，安装应用时，管理员可事先同意权限。

### <a name="best-practices-for-requesting-permissions"></a>请求权限的最佳做法
[!INCLUDE [auth-use-least-privileged](../../includes/auth-use-least-privileged.md)]

### <a name="delegated-and-application-permissions"></a>委派权限和应用程序权限
Microsoft Graph 具有两种权限类型：

- **委派权限** 由存在已登录用户的应用使用。对于这些应用，用户或管理员会同意应用请求的权限，且应用在调用 Microsoft Graph 时可以充当已登录用户。一些委派权限可以由非管理用户同意，但一些特权较高的权限需要 [管理员同意](/azure/active-directory/develop/active-directory-v2-scopes#using-the-admin-consent-endpoint)。  

- **应用程序权限** 由无需具有登录用户即可运行的应用使用；例如，作为后台服务或守护程序运行的应用。应用程序权限只能 [由管理员同意](/azure/active-directory/develop/active-directory-v2-scopes#requesting-consent-for-an-entire-tenant)。 

_有效权限_ 是应用在向 Microsoft Graph 发出请求时拥有的权限。需要了解授予应用的委派权限和应用程序权限之间的区别，以及调用 Microsoft Graph 时应用的有效权限。

- 对于委派权限，应用的有效权限是已授予应用的委派权限(通过同意)和当前已登录用户的特权的交集。应用的特权永远不能超过已登录用户。在组织内，已登录用户的特权由一个或多个管理员角色中的策略或会员资格决定。有关管理员角色的详细信息，请参阅 [在 Azure Active Directory 中分配管理员角色](/azure/active-directory/active-directory-assign-admin-roles)。<br/><br/>例如，假定已授予应用 *User.ReadWrite.All* 委派权限。此权限名义上授予应用读取和更新组织内每个用户的配置文件的权限。如果已登录用户为全局管理员，则应用可以更新组织内每个用户的配置文件。但如果已登录用户非管理员角色，则应用只能更新已登录用户的配置文件。其将不会更新组织内其他用户的配置文件，因为已登录用户不具有这些特权。

- 对于应用程序权限，应用的有效权限将是权限默示的完整级别的特权。例如，具有 *User.ReadWrite.All* 应用程序权限的应用可以更新组织中每个用户的配置文件。

:::image type="content" source="/graph/images/auth-v2/permission-types.png" alt-text="Microsoft Graph 公开了委派权限和应用程序权限，但根据应用程序的有效权限授权请求。" border="true":::

>**注意** 默认情况下，已将应用程序权限授予以下数据集的应用可访问组织中的所有邮箱：

- [日历](../permissions-reference.md#calendars-permissions)
- [联系人](../permissions-reference.md#contacts-permissions)
- [邮件](../permissions-reference.md#mail-permissions)
- [邮箱设置](../permissions-reference.md#mail-permissions)

>管理员可以配置 [应用程序访问策略](../auth-limit-mailbox-access.md)，以限制对 _特定_ 邮箱的应用访问。

有关 Microsoft Graph 委派权限和应用程序权限的完整列表，以及哪些权限需要管理员同意，请参阅 [权限参考](../permissions-reference.md)。

## <a name="getting-an-access-token"></a>获取访问令牌

和大多数开发人员一样，你可能使用身份验证库管理你的令牌与 Microsoft 标识平台的交互。身份验证库摘录了许多协议细节，例如验证、Cookie 处理、令牌缓存和保持安全连接、远离开发人员和让你关注应用上的开发情况。Microsoft 发布了开源客户端库和服务器中间件。

对于 Microsoft 标识平台终结点：

- Microsoft 身份验证库 (MSAL) 客户端库适用于 .NET、JavaScript、Android 和 Objective-C。所有平台都处于生产支持的预览下，而且，一旦引入重大更改，Microsoft 会保证升级的路径。
- 来自 Microsoft 的服务器中间件可用于 .NET core 和 ASP.NET（OWIN OpenID Connect 和 OAuth），还可用于 Node.js (Microsoft 标识平台 Passport.js)。
- Microsoft 标识平台与许多第三方身份验证库兼容。

要在完整列表中查看 Microsoft 客户端库、Microsoft 服务器中间件和兼容的第三方库，请参阅 [Microsoft 标识平台身份验证库](/azure/active-directory/develop/active-directory-v2-libraries)。

无需使用身份验证库即可获取访问令牌。 要了解如何在不使用身份验证库的情况下直接使用 Microsoft 标识平台终结点，请查看 [Microsoft 标识平台身份验证](/azure/active-directory/develop/authentication-scenarios)。

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

为帮助你快速入门，我们创建了一系列的培训模块和其他资源来展示如何在各类平台上进行身份验证和使用 API。

- 通过[使用入门](https://developer.microsoft.com/graph/get-started)页面查找你喜爱的平台所适用的库、示例、培训内容和其他资源。
- 要通过平台预配置的示例快速运行，请参阅 [Microsoft Graph 快速入门](https://developer.microsoft.com/graph/quick-start)。
- 请参阅 GitHub 上的 [Microsoft Graph 示例](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=sample&type=&language=)。

### <a name="microsoft-identity-platform-samples-and-documentation"></a>Microsoft 标识平台示例和文档

Microsoft 标识平台文档中有一些文章和示例，它们专门介绍如何向 Microsoft 标识平台进行身份验证以及如何获得它的授权。

- 最简单的起点在 [Microsoft 标识平台终结点文档](/azure/active-directory/develop/active-directory-appmodel-v2-overview) 中。本文包含概述、协议文档以及不同平台入门文章的链接，这些文章全部按你正在开发的应用类型进行整理。
- 有关使用 Microsoft 标识平台保护不同应用程序类型的示例，请查看 [Microsoft 标识平台代码示例（v2.0 终结点）](/azure/active-directory/develop/sample-v2-code)。
- 要了解客户端或服务器身份验证库列出的示例，请参阅 [Microsoft 标识平台身份验证库](/azure/active-directory/develop/active-directory-v2-libraries)。
- 在 [Azure 代码库](https://azure.microsoft.com/resources/samples/?service=active-directory)中按平台查看 Microsoft 标识平台示例。

## <a name="see-also"></a>另请参阅

- [根据方案选择 Microsoft Graph 身份验证提供程序](../sdks/choose-authentication-providers.md)
- [Microsoft 标识平台终结点文档](/azure/active-directory/develop/active-directory-appmodel-v2-overview)
