---
title: Microsoft TeamsMSAL2 提供程序
description: 使用"Teams"选项卡内的 MSAL2 Microsoft Teams，以方便身份验证和 Microsoft Graph访问所有组件。 该提供程序可用于 SSO (单一) 登录。
ms.localizationpriority: medium
author: simonagren
ms.openlocfilehash: 658c79d2b8c709c940a4db7565677ceb88c2ad12
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130607"
---
# <a name="microsoft-teams-msal2-provider"></a>Microsoft TeamsMSAL2 提供程序

使用"Microsoft Teams"选项卡内的 MSAL2 Microsoft Teams便于身份验证和 Microsoft Graph访问所有组件。 提供程序可用于 SSO 登录或 (登录) 登录。

若要了解更多信息，请参阅 [提供程序](./providers.md)。

>**提示：** 有关如何使用 Microsoft Teams MSAL2 提供程序创建 Teams 应用程序的详细信息，请参阅使用 SSO 生成 Microsoft Teams [选项卡](../get-started/build-a-microsoft-teams-tab.md)Microsoft Teams生成 [应用程序选项卡](../get-started/build-a-microsoft-teams-sso-tab.md)。


### <a name="difference-between-teams-provider-and-teams-msal2-provider"></a>MSAL2 Teams提供程序Teams差异
与 Teams 提供程序不同，Teams MSAL2 提供程序支持单一登录 (SSO) 并且构建于[msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser)上，用于客户端身份验证。 [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser)使用 PKCE 实现 OAuth 2.0 [Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow)代码。 由于授权代码Flow Web 应用程序的隐式授权Flow，因此我们建议使用 Teams MSAL2 提供程序而不是 Teams 提供程序。 有关与隐式授予流相关的安全问题的详细信息，请参阅 [隐式流的缺点](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6)。

所有新应用程序应尽可能Teams MSAL2 提供程序。 

## <a name="get-started"></a>入门

提供程序可在交互式客户端身份验证模式或 SSO 模式下使用。 

### <a name="client-side-authentication"></a>客户端身份验证
在客户端身份验证 (或交互式) ，用户首次启动应用时需要进行身份验证。 用户将需要使用登录按钮启动身份验证流程。 可以在客户端上完成此操作，并且不需要后端服务。 

### <a name="sso-authentication"></a>SSO 身份验证
为了避免要求用户向应用进行身份验证，Microsoft Teams[选项卡还可使用 SSO](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso)自动对用户进行身份验证。 但是，此过程需要后端服务，该服务用于将Microsoft Teams提供的令牌与可用于访问 Microsoft Graph 的访问令牌交换。

TeamsMSAL2 提供程序支持 SSO 模式，当设置为能够交换令牌的后端服务时 `ssoUrl`  \  `sso-url` ，将启用 SSO 模式。 后端服务需要公开 API (如) ，它将从 Microsoft Teams 接收身份验证令牌，并使用流交换令牌，获取可以访问 `api/token` Microsoft Graph 的访问令牌。 `on-behalf-of` 有关节点后端服务的参考实现，请参阅Microsoft Teams[节点 SSO 示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)。

### <a name="initialize-the-provider"></a>初始化提供程序
使用 MSAL2 Teams之前，请确保在页面中引用[Microsoft Teams SDK。](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk)

在主代码中Teams MSAL2 提供程序。

# <a name="npm"></a>[npm](#tab/ts)
在 JavaScript Teams MSAL2 提供程序时，请确保同时安装工具包和 Microsoft Teams SDK。

```cmd
npm install @microsoft/teams-js @microsoft/mgt-element @microsoft/mgt-teams-msal2-provider
```

接下来，导入并使用提供程序。

```ts
import {Providers} from '@microsoft/mgt-element';
import {TeamsMsal2Provider} from '@microsoft/mgt-teams-msal2-provider';
import * as MicrosoftTeams from "@microsoft/teams-js";

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;

Providers.globalProvider = new TeamsMsal2Provider(config);
```

其中 `config` 是

```ts
export interface TeamsMsal2Config {
  clientId: string;
  authPopupUrl: string; // see below for creating the popup page
  scopes?: string[];
  msalOptions?: Configuration;
  ssoUrl?: string; // ex: '/api/token',
  autoConsent?: boolean,
  httpMethod: HttpMethod; //ex HttpMethod.POST
}
```

# <a name="unpkg"></a>[unpkg](#tab/html)

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-msal2-provider 
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/AUTH-PATH"
  scopes="user.read,people.read..." 
  authority=""
  sso-url="/api/token" 
  http-method="POST">
></mgt-teams-msal2-provider>
```

| 属性 | 说明 |
| --- | --- |
| client-id   | 字符串客户端 ID ([配置你的Teams应用](#configure-your-teams-app)。 必填。 |
| auth-popup-url  | 将在弹出窗口中处理身份验证的页面的绝对路径或相对路径 (创建 [弹出窗口页面](#create-the-popup-page)) 。 必填。 |
| scopes  | 用户登录时必须同意的范围的逗号分隔字符串。 可选。 |
| authority    | 颁发机构字符串。 默认值为公共颁发机构。 对于单租户应用，请使用租户 ID 或租户名称。 例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` `https://login.microsoftonline.com/[your-tenant-id]` 或 。 可选。 |
| sso-url  | 处理 OBO 令牌交换的后端 API 的绝对路径或相对路径。 可选。 |
| http-method  | 用于调用后端 API 的 HTTP 方法的类型。 `POST` 或 `GET`）。 默认值为 `GET`。 可选 |

---
### <a name="create-the-popup-page"></a>创建弹出页

若要使用你的 Teams 凭据登录并处理同意，你需要提供 Teams 应用将在弹出窗口中打开的 URL，这将遵循身份验证流程。 例如，在应用程序中创建新 (，该页面将 https://mydomain.com/auth) 处理身份验证重定向并调用 `TeamsMsal2Provider.handleAuth` 方法。 这是此页面唯一需要执行的事情。 例如：

# <a name="npm"></a>[npm](#tab/ts)

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsMsal2Provider} from '@microsoft/mgt-teams-msal2-provider';

TeamsMsal2Provider.microsoftTeamsLib = MicrosoftTeams;
TeamsMsal2Provider.handleAuth();
```

# <a name="unpkg"></a>[unpkg](#tab/html)

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsMsal2Provider.handleAuth();
</script>
```
---

## <a name="configure-your-teams-app"></a>配置 Teams 应用

如果你刚开始使用应用Teams，请参阅将选项卡添加到Microsoft Teams[应用中](/microsoftteams/platform/concepts/tabs/tabs-overview)。 您还可以使用 [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) 开发应用清单。

### <a name="creating-an-appclient-id"></a>创建应用/客户端 ID

若要详细了解如何注册应用并获取交互式身份验证的客户端 ID，请参阅创建Azure Active Directory[应用](../get-started/add-aad-app-registration.md)。


若要详细了解如何注册应用并获取 SSO 的客户端 ID 和密码，请参阅使用单一登录Microsoft Teams[生成客户端 ID 和密码](../get-started/build-a-microsoft-teams-sso-tab.md)。

## <a name="migrating-from-teams-provider-to-teams-msal2-provider"></a>从 msAL2 Teams迁移到Teams MSAL2 提供程序
若要将使用 Teams 提供程序的应用程序迁移到 TEAMS MSAL2 提供程序：
1. 转到 Azure 门户，位于 https://portal.azure.com 。
1. 从菜单中，选择 **"Azure Active Directory"。**
1. 从"Azure Active Directory"菜单中，选择 **"应用注册"。**
1. 选择当前使用的应用的应用注册。 
1. 在左侧菜单上， **转到身份验证**。
1. 在 **"平台配置"** 下，**选择"添加平台**"，然后选择 **"单页应用程序"。**
1. 删除当前在 **Web** 下注册的所有重定向 URI，并改为将它们添加到 **单页应用程序 下**。
1. 在你的代码中，将 TeamsProvider 替换为Teams MSAL2 提供程序。

    如果要在 JS/TS 代码中初始化提供程序，请按照以下步骤操作：
    
    将 的 import 语句 ```mgt-teams-provider``` 替换为 
    ```ts 
    import {TeamsMsal2Provider} from '@microsoft/mgt-teams-msal2-provider';
    ```
    将 MsalProvider 的初始化替换为
    ```ts
    Providers.globalProvider = new TeamsMsal2Provider(config);
    ```
    如果以 HTML 格式初始化提供程序，请替换 
    ```html
    <mgt-teams-provider client-id="<YOUR_CLIENT_ID>" auth-popup-url="/AUTH-PATH" ... ></mgt-teams-provider>
    ``` 
    with 
    ```html
    <mgt-teams-msal2-provider client-id="<YOUR_CLIENT_ID>" auth-popup-url="/AUTH-PATH" ... ></mgt-teams-msal2-provider>
    ```

## <a name="see-also"></a>另请参阅
* [Microsoft Teams节点 SSO 示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)
* [构建 Microsoft Teams 选项卡](../get-started/build-a-microsoft-teams-tab.md)
* [使用 SSO Microsoft Teams"选项卡](../get-started/build-a-microsoft-teams-sso-tab.md)
