---
title: 获取访问令牌以调用 Microsoft Graph
description: 为了调用 Microsoft Graph，应用必须从 Microsoft 的云标识服务 Azure Active Directory (Azure AD) 获取访问令牌。
author: jackson-woods
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5438dfd81dddb2089792f37a42f87070d337a6b4
ms.sourcegitcommit: 255061099661a38278140675db4cbadbdca9be7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/07/2019
ms.locfileid: "29760919"
---
# <a name="get-access-tokens-to-call-microsoft-graph"></a>获取访问令牌以调用 Microsoft Graph

为了调用 Microsoft Graph，应用需要从 Microsoft 的云标识服务 Azure Active Directory (Azure AD) 获取访问令牌。访问令牌包含有关应用的信息（或声明）以及其具有的可通过 Microsoft Graph 使用资源和 API 的权限。若要获取一个访问令牌，应用必须能够使用 Azure AD 进行身份验证，并且用户或管理员需要获得授权以访问所需的 Microsoft Graph 资源。 

本主题概述了访问令牌、Azure AD 以及应用获取访问令牌的方式。如果你已熟悉将应用与 Azure AD 集成来获取令牌，则你可以快进到[后续步骤](#next-steps)，了解有关特定于 Microsoft Graph 的信息和示例。 

> **重要说明：** 条件访问策略应用于 Microsoft Graph 的方式正在发生变化。 应用程序需要进行更新以处理配置了条件访问策略的应用场景。 有关详细信息和指南，请参阅 [Azure Active Directory 条件访问开发人员指南](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer)。

## <a name="what-is-an-access-token-and-how-do-i-use-it"></a>什么是访问令牌以及如何使用它？

这种由 Azure AD 发布的访问令牌，称为 base 64 编码的 JSON Web 令牌 (JWT)。它们包含以下信息（声明）：Web API 受到 Azure AD 保护（如 Microsoft Graph），用于验证调用方并确保调用方有相应的权限可以执行它们正在请求的操作。当调用 Microsoft Graph 时，可以将访问令牌视为不透明。你应当随时可以通过安全通道传输访问令牌，如传输层安全性 (HTTPS)。

以下是 Azure AD 访问令牌的一个示例：

`EwAoA8l6BAAU7p9QDpi/D7xJLwsTgCg3TskyTaQAAXu71AU9f4aS4rOK5xoO/SU5HZKSXtCsDe0Pj7uSc5Ug008qTI+a9M1tBeKoTs7tHzhJNSKgk7pm5e8d3oGWXX5shyOG3cKSqgfwuNDnmmPDNDivwmi9kmKqWIC9OQRf8InpYXH7NdUYNwN+jljffvNTewdZz42VPrvqoMH7hSxiG7A1h8leOv4F3Ek/oeJX6U8nnL9nJ5pHLVuPWD0aNnTPTJD8Y4oQTp5zLhDIIfaJCaGcQperULVF7K6yX8MhHxIBwek418rKIp11om0SWBXOYSGOM0rNNN59qNiKwLNK+MPUf7ObcRBN5I5vg8jB7IMoz66jrNmT2uiWCyI8MmYDZgAACPoaZ9REyqke+AE1/x1ZX0w7OamUexKF8YGZiw+cDpT/BP1GsONnwI4a8M7HsBtDgZPRd6/Hfqlq3HE2xLuhYX8bAc1MUr0gP9KuH6HDQNlIV4KaRZWxyRo1wmKHOF5G5wTHrtxg8tnXylMc1PKOtaXIU4JJZ1l4x/7FwhPmg9M86PBPWr5zwUj2CVXC7wWlL/6M89Mlh8yXESMO3AIuAmEMKjqauPrgi9hAdI2oqnLZWCRL9gcHBida1y0DTXQhcwMv1ORrk65VFHtVgYAegrxu3NDoJiDyVaPZxDwTYRGjPII3va8GALAMVy5xou2ikzRvJjW7Gm3XoaqJCTCExN4m5i/Dqc81Gr4uT7OaeypYTUjnwCh7aMhsOTDJehefzjXhlkn//2eik+NivKx/BTJBEdT6MR97Wh/ns/VcK7QTmbjwbU2cwLngT7Ylq+uzhx54R9JMaSLhnw+/nIrcVkG77Hi3neShKeZmnl5DC9PuwIbtNvVge3Q+V0ws2zsL3z7ndz4tTMYFdvR/XbrnbEErTDLWrV6Lc3JHQMs0bYUyTBg5dThwCiuZ1evaT6BlMMLuSCVxdBGzXTBcvGwihFzZbyNoX+52DS5x+RbIEvd6KWOpQ6Ni+1GAawHDdNUiQTQFXRxLSHfc9fh7hE4qcD7PqHGsykYj7A0XqHCjbKKgWSkcAg==`

若要调用 Microsoft Graph，则将访问令牌附加为 HTTP 请求中授权标头的持有者令牌。例如，以下为返回已登录用户的个人资料信息的调用（为了不影响可读性，已截断访问令牌）：

```
HTTP/1.1
Authorization: Bearer EwAoA8l6BAAU ... 7PqHGsykYj7A0XqHCjbKKgWSkcAg==
Host: graph.microsoft.com`
GET https://graph.microsoft.com/v1.0/me/
```

## <a name="what-are-microsoft-graph-permissions"></a>Microsoft Graph 权限有哪些？
Microsoft Graph 针对其所控制的资源，公开一组丰富的粒度权限。这些权限可以表示为字符串并授权应用访问 Microsoft Graph 资源（如用户、组、用户邮件等）。例如：

- _User.Read_ 允许应用读取已登录用户的个人资料。
- _Mail.Send_ 允许应用代表已登录用户发送邮件。

有以下两种类型的权限：

- 应用所使用的的委派权限供使用当前用户运行的应用使用。将用户特权委派给代表用户调用 Microsoft Graph 的应用。其中许多权限需要用户同意，但其余权限则需要得到管理员同意。  
- 应用程序权限供不需要用户也可运行的应用使用。这些通常会在组织内授予应用广泛的特权并且始终需要管理员同意。

有关 Microsoft Graph 权限的完全列表以及委派权限和应用程序权限之间的差异，请参阅[权限引用](permissions-reference.md)。

## <a name="where-does-my-app-get-an-access-token"></a>我的应用程序从何处获取访问令牌？
应用从 Microsoft 的云标识服务 Azure Active Directory (Azure AD) 获取访问令牌。若要获取访问令牌，应用要使用 OAuth 2.0 和 OpenID Connect 1.0 规范中定义的工业标准协议与 Azure AD 交换 HTTP 请求和响应。这些协议介绍了 Azure AD 终结点并与其交换 - 或应用用于安全地使用 Azure AD 进行身份验证并获取访问令牌的身份验证流。  

简单地说，要获取访问令牌，应用要与下列终结点交换 HTTP 请求：

- `/authorize` 终结点，你的应用可在其中发送用户以使用 Azure AD 进行身份验证，并同意应用所需权限。
- `/token` 终结点，一旦获得用户同意，应用即可在其上获取访问令牌。

（注意：这些定义不是很严格。根据你的应用使用的协议，它可能会直接从 `/authorize` 终结点获取访问令牌，也可能会直接使用 `/token` 终结点进行身份验证。） 

下面是 Azure AD v2.0 公开的一组 `/authorize` 和 `/token` 终结点：

```
https://login.microsoftonline.com/common/oauth2/v2.0/authorize
https://login.microsoftonline.com/common/oauth2/v2.0/token

```
Azure AD 公开了两组终结点：Azure AD 和 Azure AD v2.0。它们之间的主要差异在于，Azure AD 终结点仅支持工作或学校帐户（即，与 Azure AD 租户相关联的帐户），而 Azure AD v2.0 支持 Microsoft 客户，如 _Live.com_ 或 _outlook.com_ 帐户。这意味着，如果使用 Azure AD 终结点，你的应用程序仅面向组织，但是使用 Azure AD v2.0 可以同时面向消费者和组织。 

Aure AD 终结点的令牌和 Azure AD v2.0 终结点的令牌不可互换，因此在开始使用生产应用前，必须在终结点之间做出选择。因为 Azure AD v2.0 终结点相对较新，而且仍在不断添加功能，需要你在做出有关在生产中为应用使用哪一个终结点的决定时考虑到某些重要的限制条件。有关详细信息，请参阅[在 Azure AD 和 Azure AD v2.0 终结点之间做选择](#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)。

## <a name="whats-the-difference-between-oauth-20-and-openid-connect"></a>OAuth 2.0 和 OpenID Connect 之间的区别是什么？

OAuth 2.0 是一个授权协议。通过使用 Azure AD 直接进行身份验证或通过 Azure AD 重定向用户来完成身份验证并同意应用请求的权限，它可以定义应用获取访问令牌的方式。在第一种情况下，应用获取其用于调用 Microsoft Graph 作为自身的访问令牌。在第二种情况下，应用获取用于代表用户调用 Microsoft Graph 的访问令牌。但是，在使用 OAuth 2.0 时，你的应用不会收到任何有关用户或 Azure AD 如何对其进行身份验证的信息。OAuth 2.0 流最常由已经知晓用户身份的移动电话或本机应用使用；或者由背景服务或守护程序这类应用使用，这类应用以其自已的身份而不是代表用户调用 Microsoft Graph。

OpenID Connect 扩展 OAuth 2.0 以提供身份层。使用 OpenID Connect，除了访问令牌以外，你的应用还可以从 Azure AD 获取 id 令牌。OpenID Connect id 令牌包含有关用户身份的声明和有关如何以及在何处对其进行身份验证的详细信息。OpenID Connect 流通常供 Web 应用使用，包括单页应用 (SPAs)。这些应用程序可以使用 id 令牌自定义其为用户请求访问令牌的行为，同时，在许多情况下，将外包其用户登录给 Azure AD 并启用单一登录 (SSO) 这种体验。

## <a name="what-kind-of-apps-can-i-call-microsoft-graph-from"></a>可以从 Microsoft Graph 调用哪种类型的应用？
你可以从以下类型的应用调用 Microsoft Graph： 

- **本机应用**：在如台式电脑、平板电脑或移动电话等设备上运行的应用。这些应用程序使用如 iOS、Android 或 Windows 这种设备上的本机操作系统 (OS) 便于用户演示和代表用户调用 Microsoft Graph。
- **Web 应用**：在服务器上运行且通过用户代理与已登录用户交互的应用通常是 Web 浏览器。在服务器上处理大多数表示层，对 Microsoft Graph 的调用则来自代表用户的服务器端。
- **单页应用 (SPA)**：Web 应用具有丰富的用户体验，可通过浏览器中的客户端脚本处理大部分表示层。对 Microsoft Graph 的调用来自使用 AJAX 这类技术和 Angular.js 这类框架的客户端脚本。代表用户进行调用。
- **后台服务/守护程序**：在没有用户存在的情况下在服务器上运行并以自已的身份调用 Microsoft Graph 的后台服务和守护程序。
- **Web API**：客户端应用调用 Web API（受 Azure AD 保护），然后 Web API 调用 Microsoft Graph，所有这些操作都以用户身份执行。受到 Azure AD 终结点支持。对于 Azure AD v2.0 终结点，只有当客户端和 Web API 具有相同的应用程序 ID 时才受支持；例如，调用 Web API 后端的本机应用。 

## <a name="how-do-i-get-my-app-talking-to-azure-ad-and-microsoft-graph"></a>如何让我的应用与 Azure AD 和 Microsoft Graph 对话？
在你的应用可以从 Azure AD 获取令牌前，必须进行注册。对于 Azure AD v2.0 终结点，请使用 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)注册你的应用。对于 Azure AD 终结点，请使用 [Azure 门户](https://portal.azure.com/)。注册会将你的应用和 Azure AD 相集成并建立其用于获取令牌的坐标和标识符。以下为：

- **应用程序 ID**：Azure AD 分配的唯一标识符。 
- **重定向 URI/URL**：应用将接收来自 Azure AD 的响应的一个或多个终结点。（对于本机和移动应用，这是由 Azure AD 分配的 URL。）
- **应用程序密码**：应用用于使用 Azure AD 进行身份验证的密码或公钥/私钥对。（对于本机或移动应用是不需要的。）

对于使用 Azure AD 终结点的应用，你还要预配置应用在注册期间需要的 Microsoft Graph 权限。对于使用 Azure AD v2.0 终结点的应用，你可能需要，也可能不需要预配置权限。 

在注册期间配置的属性可在线路上使用。例如，在以下令牌请求中：*client_id* 是*应用程序 ID*，*redirect_uri* 是应用注册的*重定向 URL* 之一，*client_secret* 则是*应用程序密码*。 

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

## <a name="are-there-authentication-libraries-available"></a>是否有可用的身份验证库？
和大多数开发人员一样，你可能将要使用身份验证库管理你与 Azure AD 的交互。身份验证库摘录了许多协议细节，如验证、cookie 处理、令牌缓存和保持安全连接、远离开发人员和让你关注应用上的开发情况。Microsoft 会为 Azure AD 和 Azure AD v2.0 终结点发布开源客户端库和服务器中间件。 

对于 Azure AD v2.0 终结点： 

- Microsoft 身份验证库 (MSAL) 客户端库适用于 .NET、JavaScript、Android 和 Objective-c。所有平台都处于生产支持的预览下，而且，一旦引入重大更改，Microsoft 会保证升级的路径。
- Microsoft 的服务器中间件适用于 .NET core 和 ASP.NET（OWIN OpenID Connect 和 OAuth），还适用于 Node.js (Microsoft Azure AD Passport.js)。 
- 此 v2.0 终结点可与多个第三方身份验证库兼容。

有关 Microsoft 客户端库、Microsoft 服务器中间件和兼容的第三方库的完整列表，请参阅 [Azure Active Directory v2.0 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries)。

对于 Azure AD 终结点：

- Active Directory 身份验证库 (ADAL) 客户端库可在数量较大的平台上使用。 
- Microsoft 的服务器中间件适用于 .NET core 和 ASP.NET 以及 Node.js。 

有关 Microsoft 客户端库和服务器中间件的完整列表，请参阅 [Azure Active Directory 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)。

## <a name="deciding-between-the-azure-ad-and-azure-ad-v20-endpoints"></a>在 Azure AD 和 Azure AD v2.0 终结点之间做选择

Azure AD 公开 Azure AD 和 Azure AD v2.0 这两组终结点，当你调用 Microsoft Graph 时，可从其中获取要使用的访问令牌。从每个终结点接收到的令牌不可互换。若要运行示例或浏览 Microsoft Graph 的功能，对 Azure AD 终结点的选择无关紧要。但是，在开始开发生产应用前，你需要确定哪一个终结点可以成为应用场景最理想的选择。下面的讨论提供了某些可以帮助你做决定的一般原则，但有关最新和最全面的信息，必须参阅 Azure Active Directory 文档中的[我应该使用 v2.0 终结点吗？](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations)。 

Azure AD 和 Azure AD v2.0 之间的主要区别在于：

* Azure AD 仅支持工作或学校帐户；即，与 Azure AD 租户关联的帐户。这意味着你的应用程序仅可面向组织。
* Azure AD v2.0 同时支持工作和学校帐户以及 Microsoft 帐户（如 _live.com_ 或 _outlook.com_ 帐户）。这意味着你的应用使用 v2.0 终结点可以同时面向消费者和组织。 

使用 Azure AD v2.0 还有某些其他优势：例如：

* 应用可在多个平台使用单一应用程序 ID。这简化了开发人员和管理员的应用管理。
* [支持动态和增量同意](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-compare#incremental-and-dynamic-consent)。通过此功能，你的应用可以在运行时请求额外的权限，将对用户同意的请求与所需功能配对。这为用户提供的体验要比首次登录时不得不同意一个很长的权限列表的体验舒适得多。  

因为 Azure AD v2.0 比 Azure AD 更新，而且仍在不断添加功能，需要你在做决定时考虑到 v2.0 终结点的某些限制条件。例如：

* 某些功能可能尚未完全在 v2.0 中实现过。例如，如果企业客户启用企业移动性安全功能，如[条件性设备访问](https://azure.microsoft.com/documentation/articles/active-directory-conditional-access-device-policies)，应用可能无法运行。
* 不可调用云解决方案提供商应用。
* [适用于联合租户的 Windows 集成身份验证](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations#limitations)不受支持。这意味着，联合 Azure AD 租户的用户不可以使用其本地 Active Directory 实例进行无提示身份验证。他们将不得不重新输入其凭据。

有关 Azure AD v2.0 终结点和 Azure AD 终结点之间的差异的详细信息，请参阅 [v2.0 终结点有何不同之处？](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-compare)。

>**重要说明**
>
>**在做出关于开发生产应用时使用哪种终结点的决定前，请参阅[我应该使用 v2.0 终结点吗？](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations)。**

## <a name="next-steps"></a>后续步骤

注册应用后，随时可以开始使用！

- 有关代表用户获取适用于调用 Microsoft Graph 的应用的访问令牌的快速步骤，请参阅[代表用户获取访问](auth-v2-user.md)。
- 有关在没有用户的情况下获取适用于调用 Microsoft Graph 的应用的访问令牌的快速步骤，请参阅[没有用户的情况下获取访问](auth-v2-service.md)。
- 若要查看你可以在 Microsoft Graph 中使用的权限，请参阅[权限](permissions-reference.md)。
- 如果你是 Microsoft 云解决方案提供商并且对通过 Microsoft Graph 访问合作伙伴托管的客户数据感兴趣，请参阅[管理应用访问 (CSPs)](auth-cloudsolutionprovider.md)。


如果你准备好跳转到代码，可以使用以下资源，帮助你在应用中使用 Azure AD 进行身份验证和授权。

### <a name="microsoft-graph-training-and-samples"></a>Microsoft Graph 培训和示例
为了帮助你快速入门，我们创建了一系列培训模块和其他资源，可向你展示如何在各种平台上验证和使用 API。 

- 使用[使用入门](https://developer.microsoft.com/zh-CN/graph/get-started)页面查找你喜爱的平台适用的库、示例、培训内容和其他资源。 
- 要使用针对平台预配置的示例快速运行，请参阅 [Microsoft Graph 快速入门](https://developer.microsoft.com/zh-CN/graph/quick-start)。
- 请参阅 GitHub 上的 [Microsoft Graph 示例](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=sample&type=&language=)。


### <a name="azure-active-directory-samples-and-documentation"></a>Azure Active Directory 示例和文档 
Azure AD 文档包含尤其关注使用 Azure AD 进行身份验证和授权的文章和示例。

对于 Azure AD v2.0 终结点： 

- [Azure AD v2.0 终结点文档](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview)是最容易开始的地方。本文包含概述链接、协议文档以及适用于所有按正在开发的应用类型组织的不同平台的入门文章。 
- 有关按客户端或服务器身份验证库列出的示例，请参阅 [Azure Active Directory v2.0 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries)。 
- 也可以通过 [Azure 代码库](https://azure.microsoft.com/resources/samples/?service=active-directory)中的平台浏览 Azure AD 示例。注意：你无法根据终结点版本限定搜索。 

对于 Azure AD 终结点： 

- [Azure AD 开发人员指南概述](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide)是最容易开始的地方。本文包含概述链接、协议文档以及适用于按正在开发的应用类型组织的不同平台的入门文章。 
- 有关按客户端或服务器身份验证库列出的示例，请参阅 [Azure Active Directory 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)。 
- 有关按应用类型和平台列出的示例，请参阅 [Azure Active Directory 代码示例](https://docs.microsoft.com/azure/active-directory/develop/active-directory-code-samples)。
- 也可以通过 [Azure 代码库](https://azure.microsoft.com/resources/samples/?service=active-directory)中的平台浏览 Azure AD 示例。注意：你无法根据终结点版本限定搜索。 


## <a name="see-also"></a>另请参阅

- [Azure Active Directory 终结点文档](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide)
- [Azure Active Directory v2.0 终结点文档](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview)
