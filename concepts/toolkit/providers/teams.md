---
title: Microsoft Teams 提供程序
description: 使用 Teams 选项卡中的 Microsoft Teams 提供程序便于进行身份验证Graph Microsoft 访问所有组件。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: b83034005a11a7ba1795b3a4e9367b4bb3e94222
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588041"
---
# <a name="microsoft-teams-provider"></a>Microsoft Teams 提供程序

使用"管理"选项卡Microsoft Teams TeamsProvider，以方便身份验证Graph Microsoft 访问所有组件。

若要了解有关身份验证提供程序的信息，请参阅 [提供程序](./providers.md)。

>**提示：** 有关如何使用 Microsoft Teams 提供程序创建 Teams 应用程序的详细信息，请参阅生成Microsoft Teams [选项卡](../get-started/build-a-microsoft-teams-tab.md)入门指南。

### <a name="difference-between-teams-provider-and-teams-msal2-provider"></a>MSAL2 Teams提供程序Teams的不同之处
与 TeamsProvider 不同，Teams MSAL2 提供程序支持单一 Sign-On (SSO) 并且基于 [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) 构建，用于客户端身份验证。 [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) 使用 PKCE 实现 OAuth 2.0 [Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow)代码。 授权代码Flow Web 应用程序的隐式授权 Flow 更安全，因此我们建议使用 Teams MSAL2 提供程序Teams提供程序。 有关与隐式授予流相关的安全问题的详细信息，请参阅 [隐式流的缺点](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6)。

所有新应用程序应尽可能Teams MSAL2 提供程序。 请参阅[Teams MSAL2 提供程序](./teams-msal2.md)了解迁移文档。

## <a name="get-started"></a>入门

使用 Teams 提供程序之前，您需要确保已在你的页面中引用 [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk)。

# <a name="npm"></a>[npm](#tab/ts)

确保同时安装工具包和 Microsoft Teams SDK。

```cmd
npm install @microsoft/mgt @microsoft/teams-js
```

接下来，导入并使用提供程序。

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

其中 `config` 是

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string; // see below for creating the popup page
  scopes?: string[];
  msalOptions?: Configuration;
}
```

# <a name="unpkg"></a>[unpkg](#tab/html)

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/AUTH-PATH"
  scopes="User.Read,People.Read..."
  authority=""
></mgt-teams-provider>
```

### <a name="mgt-teams-provider-attributes"></a>mgt-teams-provider 属性
| 属性 | 说明 |
| --- | --- |
| client-id   | 字符串客户端 ID ([配置你的Teams应用](#configure-your-teams-app)。 必需项。 |
| auth-popup-url  | 将在弹出窗口中处理身份验证的页面的绝对路径或相对路径 (创建 [弹出窗口页面](#create-the-popup-page)) 。 必需项。 |
| scopes  | 用户登录时必须同意的范围的逗号分隔字符串。 可选。 |
| depends-on | 另一个优先级较高的提供程序组件的元素选择器字符串。 可选。 |
| authority    | 颁发机构字符串。 默认值为公共颁发机构。 对于单租户应用，请使用租户 ID 或租户名称。 例如，`https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` 或 `https://login.microsoftonline.com/[your-tenant-id]`。 可选。 |

---

### <a name="create-the-popup-page"></a>创建弹出页

为了使用 Teams 凭据登录，你需要提供 Teams 应用将在弹出窗口中打开的 URL，这将遵循身份验证流程。 此 URL 需要在你的域中，并且它需要调用 `TeamsProvider.handleAuth();` 方法。 这是此页面唯一需要执行的事情。 例如：

# <a name="npm"></a>[npm](#tab/ts)

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
TeamsProvider.handleAuth();
```

# <a name="unpkg"></a>[unpkg](#tab/html)

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```
---

### <a name="configure-redirect-uris"></a>配置重定向 URI

在网站上发布弹出窗口后，您需要使用 属性中的 `auth-popup-url/authPopupUrl` URL。 还需要在应用门户的应用配置中，将此 URL 配置为Azure AD URI。

## <a name="configure-your-teams-app"></a>配置 Teams 应用

如果你刚开始使用应用Teams，请参阅[将选项卡添加到Microsoft Teams应用中](/microsoftteams/platform/concepts/tabs/tabs-overview)。 您还可以使用 [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) 快速开发应用清单。
### <a name="creating-an-appclient-id"></a>创建应用/客户端 ID
若要获取客户端 ID，需要在客户端 ID 中[注册](../get-started/add-aad-app-registration.md)Azure AD。 
>**注意**：MSAL 仅支持 OAuth Flow隐式类型。 请确保在 Azure 门户Flow应用程序中启用隐式 (默认情况下未启用隐式) 。 在 **"** 身份验证"下，找到 **"隐式** 授予"部分，并选中" **访问** 令牌和 **ID 令牌"的复选框**。 

## <a name="see-also"></a>另请参阅
* [Microsoft Teams选项卡示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)
* [构建 Microsoft Teams 选项卡](../get-started/build-a-microsoft-teams-tab.md)
