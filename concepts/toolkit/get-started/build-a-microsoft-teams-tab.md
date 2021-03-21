---
title: 使用 Microsoft Graph 工具生成 Microsoft Teams Toolkit
description: 开始使用 Microsoft Graph 工具生成 Microsoft Teams Toolkit。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 915bbe562fec9ef0bcbd5ae6d67d8497ea7e72eb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963272"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph 工具生成 Microsoft Teams Toolkit

本主题介绍如何开始在 Microsoft Teams 解决方案Toolkit Microsoft Graph 应用。 入门包括以下步骤：

1. 使用自定义选项卡创建新的 Teams 应用程序。
2. 添加 Microsoft Graph Toolkit。
3. 初始化 Microsoft Teams 提供程序。
4. 创建身份验证弹出窗口页面。
5. 添加组件。
6. 测试你的应用。

## <a name="create-a-new-teams-application-with-a-custom-tab"></a>使用自定义选项卡创建新的 Teams 应用程序

创建新 Teams 应用的最简单方法是使用 [Microsoft Teams](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) Toolkit扩展进行Visual Studio代码。 按照说明 [设置新的 Teams 项目](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project)。 When you get to the **Add capabilities** screen， select **Tab**， and then **Personal tab**.

## <a name="add-the-microsoft-graph-toolkit"></a>添加 Microsoft Graph Toolkit

可以在应用程序中使用 Microsoft Graph Toolkit，方法为通过 unpkg (直接引用加载程序) 安装 npm 包。 若要使用Toolkit，你还需要 [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)。

### <a name="use-via-mgt-loader"></a>通过 mgt-loader 使用
若要通过Toolkit使用 Toolkit 和 Teams SDK，在 文件中添加以下 `<head>` `public/index.html` 引用：

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>通过 npm (ES6 模块) 
通过 ES6 模块Toolkit可完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。 若要使用 ES6 模块，请为项目添加 Toolkit 和 Microsoft Teams SDK 的 npm 包：

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a>初始化 Teams 提供商

Microsoft Graph Toolkit提供程序支持对组件的 Microsoft Graph 进行身份验证和访问。 若要了解更多信息，请参阅 [使用提供程序](../providers/providers.md)。 [Teams 提供程序](../providers/teams.md)处理所有需要通过 Teams SDK 实现以对用户进行身份验证的逻辑和交互。

可以选择在 HTML 或 JavaScript 代码中初始化提供程序。 

### <a name="initialize-in-html"></a>在 HTML 中初始化

在 `public/index.html` 中，将 Teams 提供商添加到 `<body>` 中，如下所示。

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/auth.html"
></mgt-teams-provider>
```

将 `<YOUR_CLIENT_ID>` 替换为应用程序的客户端 ID。 

### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化

若要在 JavaScript 代码中初始化提供程序，请在 `src/components/App.js` 项目目录中找到文件。 导入 Teams 提供商并初始化提供商。

```js
import * as microsoftTeams from "@microsoft/teams-js";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
将 `<YOUR_CLIENT_ID>` 替换为应用程序的客户端 ID。

### <a name="creating-an-appclient-id"></a>创建应用/客户端 ID

若要获取客户端 ID，需要注册 Azure Active Directory 应用程序。 按照创建 Azure [Active Directory 应用文章中的步骤](./add-aad-app-registration.md) 操作。

请确保在应用注册中将重定向 **URI** 设置为指向 `auth.html` 你的页面。 例如，如果你正在 上运行你的应用， `localhost:3000` 将重定向 URI 设置为 `https://localhost:3000/auth.html` 。

>**注意**：MSAL 仅支持 OAuth 的隐式流。 请确保在 Azure 门户应用程序中启用隐式流 (默认情况下不会启用它) 。 在 **身份验证** 下，找到 **隐式授予** 部分，并选中 **访问** 令牌和 **ID 令牌的复选框**。 

## <a name="create-the-auth-popup-page"></a>创建身份验证弹出页

为了允许用户登录，你需要提供 Teams 应用将在弹出窗口中打开的 URL，以遵循身份验证流程。 URL 需要位于域中，此页面需要执行的所有操作就是调用 `TeamsProvider.handleAuth()` 方法。

为此，可以在文件夹中添加一个新文件 (该文件应处于与) 相同的级别，并 `auth.html` `public` `index.html` 添加以下代码： 

```html
<!DOCTYPE html>
<html>
  <head>
    <script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
    <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
  </head>

  <body>
    <script>
      mgt.TeamsProvider.handleAuth();
    </script>
  </body>
</html>
```

## <a name="add-components"></a>添加组件

现在，你已准备好将任何 Microsoft Graph Toolkit组件添加到你的选项卡。 

您可以像平常一样向 HTML 添加组件。 例如，若要添加 Login 组件，将以下代码添加到 的正文 `index.html` 中：

```html
<mgt-login></mgt-login>
```

或者，可以将 JSX 中的组件添加到选项卡组件。 如果你使用 Microsoft Teams 应用扩展创建了 Teams 应用，我们建议 `mgt-react` Toolkit库。 若要了解更多信息，请参阅 [将 Microsoft Graph Toolkit React](./use-toolkit-with-react.md)

首先，安装 `mgt-react` ：

```bash
npm install @microsoft/mgt-react
```

找到 `src/components/Tab.js` 文件，然后从库导入想要使用 `mgt-react` 的组件。 例如，若要添加 `Login` 组件，请使用：

```js
import { Login } from "@microsoft/mgt-react"
```

然后，将组件添加到 方法的 `return()` `render()` 语句 `Tab` 中：

```jsx
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a>测试应用程序

使用下列命令生成并运行应用程序：
```bash
npm install
npm start
```

若要测试应用程序，可以通过 Teams Toolkit 扩展将应用安装到 Teams。 打开 Teams Toolkit 扩展，然后单击 **"打开 Microsoft Teams Toolkit"。** 单击 **左侧菜单中的 App Studio，** 向下滚动并选择测试和 **分发，然后****安装**。 Teams 将在浏览器中打开，并且你将被重定向到你创建的选项卡。 你应该能够看到登录组件，并使用它登录到你的应用程序。

## <a name="next-steps"></a>后续步骤
- 请查看此有关生成 Teams 选项卡 [的分步教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)。
- 尝试在运动场中的 [组件](https://mgt.dev)。
- 在 Stack [Overflow 上提问](https://aka.ms/mgt-question)。
- 在 GitHub 上报告 Bug 或保留 [功能请求](https://aka.ms/mgt)。
