---
title: 使用 Microsoft Microsoft Teams生成一个"Graph Toolkit
description: 开始 Microsoft Microsoft Teams生成一个Graph Toolkit。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 6b33fda93f3383fede93d79362762ea234e7a8be
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589014"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Microsoft Teams生成一个"Graph Toolkit

本主题介绍如何开始在解决方案Graph Toolkit Microsoft Microsoft Teams Microsoft 应用程序。 本指南适用于在 SSO 应用中没有单一登录 (单页) 不需要后端。 如果要使用自定义后端实现 SSO，请参阅使用 SSO Microsoft Teams生成 ([选项卡) ](./build-a-microsoft-teams-sso-tab.md)。

生成选项卡涉及以下步骤：

1. 添加 Microsoft Graph Toolkit。
1. 创建身份验证弹出窗口页面。
1. 创建应用/客户端 ID
1. 初始化 MSAL2 Teams。
1. 添加组件。
1. 测试你的应用。

## <a name="add-the-microsoft-graph-toolkit"></a>添加 Microsoft Graph Toolkit

可以在应用程序中使用 Microsoft Graph Toolkit，方法为直接通过 unpkg (加载程序) 安装 npm 包。 若要使用Toolkit，你还需要 Microsoft Teams [SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk)。

# <a name="unpkg"></a>[unpkg](#tab/unpkg)
若要通过Toolkit使用 Teams SDK，请向代码添加脚本中的引用：

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

# <a name="npm"></a>[npm](#tab/npm)
通过 ES6 模块使用工具包可以完全控制捆绑过程，并允许仅捆绑应用程序所需的代码。 若要使用 ES6 模块，请为项目添加 Toolkit 和 Microsoft Teams SDK 的 npm 包：

```cmd
npm install @microsoft/teams-js @microsoft/mgt-element @microsoft/mgt-teams-msal2-provider @microsoft/mgt-components
```

---

## <a name="create-the-auth-popup-page"></a>创建身份验证弹出页

为了允许用户登录，你需要在应用中打开一个页面Teams弹出窗口中打开该页面以遵循身份验证流。 页面的路径可以是任何内容，只要它位于你的应用应用路径 (例如， https://yourdomain.com/tabauth)。 此页面的唯一要求是调用 方法 `TeamsMsal2Provider.handleAuth()` ，但您可以添加任何内容或加载您想要的进度。

下面是处理弹出窗口中的身份验证流的基本页面示例。

# <a name="unpkg"></a>[unpkg](#tab/unpkg)
```html
<!DOCTYPE html>
<html>
  <head>
    <script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
    <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
  </head>

  <body>
    <script>
      mgt.TeamsMsal2Provider.handleAuth();
    </script>
  </body>
</html>
```
# <a name="npm"></a>[npm](#tab/npm)
```js
import { TeamsMsal2Provider } from '@microsoft/mgt-teams-msal2-provider';

TeamsMsal2Provider.handleAuth();
```

---

## <a name="creating-an-appclient-id"></a>创建应用/客户端 ID
若要获取客户端 ID，您需要注册一个Azure Active Directory应用程序。 按照创建应用[应用Azure Active Directory中的步骤](./add-aad-app-registration.md)操作。

请确保在应用 `redirect URI` 注册中将 设置为指向你在上一步中创建的身份验证页面。 例如，https://localhost:3000/tabauth。

> **注意：** 请确保将 设置为 `redirect URI` `Single Page Application (SPA)`。 Teams MSAL2 提供程序在后台使用 MSAL2 提供程序。

## <a name="initialize-the-teams-msal2-provider"></a>初始化 MSAL2 Teams

Microsoft Graph 工具包提供程序为组件启用身份验证和对 Microsoft Graph 的访问。 若要了解详细信息，请参阅[使用提供程序](../providers/providers.md)。 MSAL2 提供程序Teams [MSAL2](../providers/teams-msal2.md) 提供程序处理需要通过 Teams SDK 实现以对用户进行身份验证的所有逻辑和交互。

可以选择在 HTML 或 JavaScript 代码中初始化提供程序。 

# <a name="html"></a>[html](#tab/html)


将组件 `mgt-teams-msal2-provider` 添加到 HTML 页面，如下所示。

```html
<mgt-teams-msal2-provider 
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/tabauth"
  scopes="User.Read,Mail.ReadBasic"
  ></mgt-teams-msal2-provider>
```

将 `<YOUR_CLIENT_ID>` 替换为应用程序的客户端 ID，将 替换为 `auth-popup-url` 身份验证页面的完整路径或相对路径。 

# <a name="js"></a>[js](#tab/js)


若要在 JavaScript 代码中初始化提供程序，请向应用程序添加以下代码：

```ts
import {Providers} from '@microsoft/mgt-element';
import {TeamsMsal2Provider} from '@microsoft/mgt-teams-msal2-provider';
import * as MicrosoftTeams from "@microsoft/teams-js";

TeamsMsal2Provider.microsoftTeamsLib = MicrosoftTeams;

Providers.globalProvider = new TeamsMsal2Provider({
  clientId: `<YOUR_CLIENT_ID>`,
  authPopupUrl: '/tabauth',
  scopes: ['User.Read','Mail.ReadBasic'],
});
```
将 `<YOUR_CLIENT_ID>` 替换为应用程序的客户端 ID，将 替换为 `authPopupUrl` 身份验证页面的完整路径或相对路径。

---
## <a name="add-components"></a>添加组件

现在，你已准备好添加任何 Microsoft Graph Toolkit组件。 可能需要添加的第一个组件是登录组件。

```HTML
<mgt-login></mgt-login>
```

登录组件呈现"登录"按钮，该按钮将指导用户完成登录过程，并集成任何提供程序以处理身份验证。 用户登录后，所有其他工具包组件将能够自动调用 Microsoft Graph。 提供程序还会公开经过身份验证的 Microsoft Graph客户端，以执行 API 调用或获取访问令牌。 有关详细信息，请参阅 [使用提供程序](../providers/providers.md)。

如果你使用的是 React，我们建议改为React库中的组件`mgt-react`。 若要了解更多信息，请参阅[将 Microsoft Graph Toolkit与 React](./use-toolkit-with-react.md)

## <a name="next-steps"></a>后续步骤
- 在[样本](https://mgt.dev)中试用组件。
- 在 [Microsoft 问答中&问题](/answers/topics/microsoft-graph-toolkit.html)。
- 在 [GitHub](https://aka.ms/mgt) 上报告 bug 或提出功能请求。
- 请查看Microsoft Teams[示例](https://github.com/OfficeDev/Microsoft-Teams-Samples/tree/main/samples/tab-graph-toolkit)。
