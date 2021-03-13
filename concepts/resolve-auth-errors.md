---
title: 解决 Microsoft Graph 授权错误
description: 了解如何解决 Microsoft Graph 401 和 403 授权错误。
author: davidmu1
localization_priority: Priority
ms.prod: applications
ms.openlocfilehash: 13e815b72157da2fe5d8db8114a3dac436b40026
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760937"
---
# <a name="resolve-microsoft-graph-authorization-errors"></a>解决 Microsoft Graph 授权错误

授权错误可能是由多个不同的问题造成的，其中大多数问题会产生 403 错误(有几个例外)。 例如，以下情况可能会导致授权错误：

* 不正确的[访问令牌获取流](/azure/active-directory/develop/active-directory-authentication-scenarios)
* 配置不当的[权限范围](/azure/active-directory/develop/active-directory-v2-scopes)
* 缺乏[许可](/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)
* 缺少[权限](/azure/active-directory/develop/v2-permissions-and-consent)

## <a name="steps-to-resolve-common-errors"></a>解决常见错误的步骤

若要解决常见授权错误，请尝试针对与你遇到的错误最接近的错误描述的步骤。 可能会出现多个错误。 你还可以查看 Microsoft Q&A 上已有的 [401 错误](https://docs.microsoft.com/answers/search.html?c=&includeChildren=&f=&type=question+OR+idea+OR+kbentry+OR+answer+OR+topic+OR+user&redirect=search%2Fsearch&sort=relevance&q=%5Bmicrosoft-graph%5D%20401%20)和 [403 错误](https://docs.microsoft.com/answers/search.html?c=&includeChildren=&f=&type=question+OR+idea+OR+kbentry+OR+answer+OR+topic+OR+user&redirect=search%2Fsearch&sort=relevance&q=%5Bmicrosoft-graph%5D%20403)相关的答案。 如果无法找到解决问题的方法，请在 [Microsoft Q&A](https://aka.ms/askgraph) 上提问并标记为 *microsoft-graph**。

**401 未授权错误：你的令牌是否有效？** <br>

请确保你的应用程序在请求中向 Microsoft Graph 提供有效的访问令牌。 此错误通常意味着 HTTP 身份验证请求标头中缺少访问令牌，或者令牌无效或已过期。 强烈建议使用 [Microsoft 身份验证库 (MSAL)](/azure/active-directory/develop/msal-overview) 获取访问令牌。 此外，如果你尝试使用授予个人 Microsoft 帐户的委派访问令牌来访问仅支持工作或学校帐户（组织帐户）的 API，则可能会发生此错误。 

**403 禁止错误：你是否选择了正确的权限集？**<br>

根据您的应用调用的 Microsoft Graph API，验证你是否请求了正确的权限集。 所有 Microsoft Graph API 方法参考主题中都提供了我们建议的最低特权权限。 此外，这些权限必须由用户或管理员向应用程序授予。 授予权限通常通过同意页进行，也可使用 Azure 门户应用程序注册边栏选项卡授予权限。 从应用程序的“**设置**”边栏选项卡，单击“**所需权限**”，然后单击“**授予权限**”。 <br>

* [Microsoft Graph 权限](./permissions-reference.md) <br>
* [了解 Azure AD 权限和许可](/azure/active-directory/develop/v2-permissions-and-consent) <br>

**403 禁止错误：你的应用是否获取了与所选权限匹配的令牌？** <br>

确保请求或授予的权限类型与你的应用获取的访问令牌类型相匹配。 你可能正在请求和授予应用程序权限，但使用的是委派的交互式代码流令牌而不是客户端凭据流令牌，或者正在请求和授予委派权限，但使用的是客户端凭据流令牌而不是委派的代码流令牌。 <br>
* [代表用户获取访问权限和委派权限](/graph/auth_v2_user) 
* [Azure AD v2.0 - OAuth 2.0 授权代码流](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
* [在没有用户的情况下获取访问权限（守护程序服务）和应用程序权限](/graph/auth_v2_service)
* [Azure AD v2.0 - OAuth 2.0 客户端凭据流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 禁止访问错误：重置密码** <br>

目前，没有应用程序权限守护程序服务到服务权限允许重置用户密码。 这些 API 仅支持对登录的管理员使用交互式委派代码流。

* [Microsoft Graph 权限](./permissions-reference.md) <br>

**403 禁止：用户是否具有访问权限，是否获得许可？** <br>

对于委派代码流，Microsoft Graph 将根据向应用授予的权限以及登录用户具有的权限来评估是否允许请求。 通常，此错误表示用户没有足够的特权执行请求 **或者** 用户没有获得所访问数据的许可。 只有具有所需权限或许可证的用户才能成功发出请求。

**403 禁止：是否选择了正确的资源 API？** <br>

API 服务（如 Microsoft Graph）检查接收的访问令牌中的 *aud* 声明 (audience) 是否与预期值匹配，如果不匹配，则会导致 `403 Forbidden` 错误。 导致此错误的常见错误是尝试使用为 Azure AD Graph API、Outlook API 或 SharePoint/OneDrive API 获取的令牌调用 Microsoft Graph（或反之）。 确保你的应用为其获取令牌的资源（或范围）与应用调用的 API 匹配。

**400 错误请求或 403 禁止：用户是否符合其组织的条件访问 (CA) 策略？**<br>

根据组织的 CA 策略，通过你的应用访问 Microsoft Graph 资源的用户可能会被要求提供附加信息，而这些信息在你的应用最初获取的访问令牌中并不存在。 在这种情况下，你的应用在获取访问令牌期间会收到 400 以及 *interaction_required* 错误，或者在调用 Microsoft Graph 时收到 403 以及 *insufficient_claims* 错误。 在这两种情况下，错误响应都包含可呈现给授权终结点的附加信息，以便向用户质询其他信息（如多重身份验证或设备注册）。

* [使用 MSAL 处理条件访问质询](/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
* [Azure Active Directory 条件访问开发人员指南](/azure/active-directory/develop/conditional-access-dev-guide)