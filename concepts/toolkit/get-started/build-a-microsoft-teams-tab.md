---
title: 使用 Microsoft Microsoft Teams生成一个"Graph Toolkit
description: 开始使用 Microsoft Microsoft Teams生成 Graph Toolkit。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 1751214a354de77edfdf730463320caf5d963a27c6cc47b553f20b61aaaa71d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54143603"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Microsoft Teams生成一个"Graph Toolkit

本主题介绍如何开始在解决方案Graph Toolkit Microsoft Microsoft Teams Microsoft 解决方案。 开始使用涉及以下步骤：

1. 使用自定义选项卡Teams应用程序。
2. 添加 Microsoft Graph Toolkit。
3. 初始化Microsoft Teams提供程序。
4. 创建身份验证弹出窗口页面。
5. 添加组件。
6. 测试你的应用。

## <a name="create-a-new-teams-application-with-a-custom-tab"></a>使用自定义选项卡Teams应用程序

创建新应用的最简单方法是Teams应用Microsoft Teams Toolkit[扩展](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension)Visual Studio Code。 按照说明[设置新的项目Teams项目](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project)。 When you get to the **Add capabilities** screen， select **Tab**， and then **Personal tab**.

## <a name="add-the-microsoft-graph-toolkit"></a>添加 Microsoft Graph Toolkit

可以在应用程序中使用 Microsoft Graph Toolkit，方法为通过 unpkg (直接引用加载程序) 安装 npm 包。 若要使用Toolkit，你还需要使用[Microsoft Teams SDK。](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)

### <a name="use-via-mgt-loader"></a>通过 mgt-loader 使用
若要通过Toolkit使用 Teams SDK，在 文件中添加以下 `<head>` `public/index.html` 引用：

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>通过 npm (ES6 模块) 
通过 ES6 模块使用 Toolkit 可以完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。 若要使用 ES6 模块，请为项目添加 Toolkit 和 Microsoft Teams SDK 的 npm 包：

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a>初始化Teams提供程序

Microsoft Graph 工具包提供程序为组件启用身份验证和对 Microsoft Graph 的访问。 若要了解详细信息，请参阅[使用提供程序](../providers/providers.md)。 Teams[提供程序](../providers/teams.md)处理所有需要通过 Teams SDK 实现的逻辑和交互来对用户进行身份验证。

可以选择在 HTML 或 JavaScript 代码中初始化提供程序。 

### <a name="initialize-in-html"></a>在 HTML 中初始化

在 `public/index.html` 中，Teams提供程序添加到 `<body>` 中，如下所示。

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/auth.html"
></mgt-teams-provider>
```

将 `<YOUR_CLIENT_ID>` 替换为应用程序的客户端 ID。 

### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化

若要在 JavaScript 代码中初始化提供程序，请在 `src/components/App.js` 项目目录中找到文件。 导入Teams提供程序并初始化提供程序。

```JavaScript
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

若要获取客户端 ID，您需要注册一个Azure Active Directory应用程序。 按照创建应用[应用Azure Active Directory中的步骤](./add-aad-app-registration.md)操作。

请确保在应用注册中将重定向 **URI** 设置为指向 `auth.html` 你的页面。 例如，如果你正在 上运行你的应用， `localhost:3000` 将重定向 URI 设置为 `https://localhost:3000/auth.html` 。

>**注意**：MSAL 仅支持 OAuth Flow隐式身份验证。 请确保在 Azure 门户Flow在应用程序中启用隐式 (默认不启用隐式) 。 在 **身份验证** 下，找到 **隐式授予** 部分，并选中 **访问** 令牌和 **ID 令牌的复选框**。 

## <a name="create-the-auth-popup-page"></a>创建身份验证弹出页

为了允许用户登录，你需要提供一个 URL，Teams应用将在弹出窗口中打开该 URL 以遵循身份验证流。 URL 需要位于域中，此页面需要执行的所有操作就是调用 `TeamsProvider.handleAuth()` 方法。

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

```HTML
<mgt-login></mgt-login>
```

或者，可以将 JSX 中的组件添加到选项卡组件。 如果你使用 Microsoft Teams Toolkit 扩展创建了 `mgt-react` Teams 应用，我们建议Microsoft Teams Toolkit库。 若要了解更多信息，请参阅[将 Microsoft Graph Toolkit与 React](./use-toolkit-with-react.md)

首先，安装 `mgt-react` ：

```Command Line
npm install @microsoft/mgt-react
```

找到 `src/components/Tab.js` 文件，然后从库导入想要使用 `mgt-react` 的组件。 例如，若要添加 `Login` 组件，请使用：

```JavaScript
import { Login } from "@microsoft/mgt-react"
```

然后，将组件添加到 方法的 `return()` `render()` 语句 `Tab` 中：

```JavaScript
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

若要测试应用程序，可以通过 Teams Extension 将应用Teams Toolkit应用。 打开"Teams Toolkit扩展"，然后单击"**打开Microsoft Teams Toolkit"。** 单击 **左侧菜单中的 App Studio，** 向下滚动并选择测试和 **分发，然后****安装**。 Teams将在浏览器中打开，并且你将被重定向到你创建的选项卡。 你应该能够看到登录组件，并使用它登录到你的应用程序。

## <a name="next-steps"></a>后续步骤
- 请查看此分步教程，介绍如何生成Teams[选项卡](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)。
- 在[样本](https://mgt.dev)中试用组件。
- 在 [Stack Overflow](https://aka.ms/mgt-question) 上提问。
- 在 [GitHub](https://aka.ms/mgt) 上报告 bug 或提出功能请求。
