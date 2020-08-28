---
title: Microsoft Teams 提供程序
description: 使用 Microsoft "团队" 选项卡中的团队提供程序来促进对所有组件的身份验证和 Microsoft Graph 访问。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 39a20b3946a795af34fd57d877214a9cb7dabcae
ms.sourcegitcommit: 4a37678913c98f62b8174de6ca03908b9af864bd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/28/2020
ms.locfileid: "47296482"
---
# <a name="microsoft-teams-provider"></a>Microsoft Teams 提供程序

使用 Microsoft "团队" 选项卡中的团队提供程序来促进对所有组件的身份验证和 Microsoft Graph 访问。

若要了解详细信息，请参阅 [提供程序](../providers.md)。

## <a name="get-started"></a>入门

在使用团队提供程序之前，您需要确保您已在页面中引用 [Microsoft 团队 SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) 。

### <a name="via-script-tag"></a>via script 标记
下面的示例通过 CDN) 在 HTML (中使用提供程序。

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR-DOMAIN>.com/AUTH-PATH"
  authority=""
></mgt-teams-provider>
```

| 属性 | 说明 |
| --- | --- |
| 客户端 id   | 字符串客户端 ID (请参阅 [配置团队应用程序](#configure-your-teams-app)。 必需项。 |
| auth-popup-url  | 将在弹出窗口中处理 auth 的页面的绝对或相对路径 (请参阅 [Create the popup page](#create-the-popup-page)) 。 必需项。 |
| scopes  | 用户必须同意登录时的作用域的逗号分隔字符串。 可选。 |
| 取决于 | 另一个较高优先级提供程序组件的元素选择器字符串。 可选。 |
| 监管    | 颁发机构字符串。 默认值是公共颁发机构。 对于单租户应用，请使用租户 ID 或租户名称。 例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` 或 `https://login.microsoftonline.com/[your-tenant-id]` 。 可选。 |


### <a name="via-npm"></a>via NPM
下面的示例通过 NPM) 在 JS 模块中使用提供程序 (。

请务必同时安装工具包和 Microsoft 团队 SDK。

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

接下来，导入并使用提供程序。

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt';
Providers.globalProvider = new TeamsProvider(config);
```

其中 `config` 是

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

或者，您可能需要设置对 Microsoft 团队库的引用。 如以下示例所示：

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

有关完整示例，请参阅 [Microsoft 团队选项卡示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)。

## <a name="configure-your-teams-app"></a>配置团队应用程序

如果只是开始使用团队应用程序，请参阅 [将选项卡添加到 Microsoft 团队应用](/microsoftteams/platform/concepts/tabs/tabs-overview)。 您还可以使用 [应用程序 Studio](/microsoftteams/platform/get-started/get-started-app-studio) 快速开发您的应用程序清单。

使用选项卡安装您的应用程序并准备好使用组件时，需要确保您的应用程序具有访问 Microsoft Graph 的适当权限。 若要使用所需的权限配置应用程序，请执行以下操作：

1. [检索你的域名](/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [创建新的应用注册](/azure/active-directory/identity-protection/graph-get-started#create-a-new-app-registration)
3. [授予应用程序权限](/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

在 " **添加 API 访问" 页**上添加正确的权限非常重要。 你将需要管理员添加和批准权限，具体取决于所需的组件。

>**提示：** 如果你不确定要添加哪些权限，请参阅每个组件的文档。

### <a name="enable-implicit-grant-flow"></a>启用隐式授予流

请确保启用隐式授予流;这对于从客户端请求令牌的 web 应用程序是必需的。 在 Azure 门户中，在管理应用注册时，请编辑清单并更改 `oauth2AllowImplicitFlow` 为 `true` 。

### <a name="create-the-popup-page"></a>创建弹出页

若要使用你的团队凭据登录，你需要提供团队应用将在弹出项中打开的 URL，这将遵循身份验证流。 此 URL 必须在您的域中，并且需要调用该 `TeamsProvider.handleAuth();` 方法。 这是此页面唯一需要执行的操作。 例如：

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

或通过身份验证弹出页面中引用的模块：

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
TeamsProvider.handleAuth();
```

### <a name="configure-redirect-uris"></a>配置重定向 Uri

在您的网站上发布此页面后，您需要使用属性中的 URL `auth-popup-url/authPopupUrl` 。 此外，还需要在 Azure AD 门户的应用配置中将此 URL 配置为有效的重定向 URI。
