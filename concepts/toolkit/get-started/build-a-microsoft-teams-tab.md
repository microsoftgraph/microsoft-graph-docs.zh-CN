---
title: 使用 Microsoft Graph 工具生成 Microsoft Teams Toolkit
description: 开始使用 Microsoft Graph 选项卡生成 Microsoft Teams Toolkit。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 9cd548e78ff21577df852a28be76e45144bfb91d
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663916"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph 工具生成 Microsoft Teams Toolkit

本主题介绍如何开始在 Microsoft Teams 解决方案Toolkit Microsoft Graph 应用程序。 入门包括以下步骤：

1. 使用自定义选项卡创建新的 Teams 应用程序。
2. 设置 ngrok 并创建隧道。
3. 添加 Microsoft Graph Toolkit。
4. 初始化 Microsoft Teams 提供程序。
5. 创建身份验证弹出窗口。
6. 添加组件。
7. 测试你的应用。

## <a name="create-a-new-teams-application-with-a-custom-tab"></a>使用自定义选项卡创建新的 Teams 应用程序

创建新 Teams 应用的最简单方法是使用 Microsoft Teams Toolkit [扩展Visual Studio](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) 代码。 按照说明 [设置新的 Teams 项目](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project)。 当你进入"添加 **功能** "屏幕时，选择 **"选项卡**"，然后选择"个人 **"选项卡**。

## <a name="set-up-ngrok-and-create-a-tunnel"></a>设置 ngrok 并创建隧道

为了稍后测试应用程序，您需要使用 HTTPS 通过面向公众的 URL 承载应用程序。 通过 [以下命令安装 ngrok](https://ngrok.com/download) 并创建从 Internet 到 localhost：3000 的隧道：

```bash
ngrok http 3000
```
在项目目录中，找到 `.publish\Development.env` 该文件，并将其值替换为 `baseUrl0` ngrok URL。

## <a name="add-the-microsoft-graph-toolkit"></a>添加 Microsoft Graph Toolkit

可以在应用程序中使用 Microsoft Graph Toolkit，方法为直接通过取消 (加载程序) 安装 npm 包。 若要使用Toolkit，你还需要[Microsoft Teams SDK。](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)

### <a name="use-via-mgt-loader"></a>通过 mgt-loader 使用
若要通过Toolkit使用 Toolkit 和 Teams SDK，请添加以下引用 `public/index.html` ：

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>通过 npm (ES6 模块) 
通过 ES6 模块使用 Toolkit 可完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。 若要使用 ES6 模块，请为项目添加 Toolkit 和 Microsoft Teams SDK 的 npm 包：

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a>初始化 Teams 提供商

Microsoft Graph Toolkit提供程序为组件启用身份验证并访问 Microsoft Graph。 若要了解更多信息，请参阅["使用提供程序"。](../providers/providers.md) [Teams 提供程序](../providers/teams.md)处理需要通过 Teams SDK 实现以对用户进行身份验证的所有逻辑和交互。

可以选择在 HTML 或 JavaScript 代码中初始化提供程序。 

### <a name="initialize-in-html"></a>使用 HTML 进行初始化

In `public/index.html` ， add the Teams provider as shown.

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

用 `<YOUR_CLIENT_ID>` 应用程序的客户端 ID 和您 `<YOUR_NGROK_URL>` 创建的 ngrok URL 替换。

### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化

若要在 JavaScript 代码中初始化提供程序，请在 `src/components/App.js` 项目目录中找到该文件。 导入 Teams 提供商并初始化提供商。

```js
import * as microsoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
替换为 `<YOUR_CLIENT_ID>` 应用程序的客户端 ID。

### <a name="creating-an-appclient-id"></a>创建应用/客户端 ID
若要获取客户端 ID，需要在 Azure AD 中 [注册](../../auth-register-app-v2.md) 应用程序。 请确保将具有身份验证弹出窗口完整路径的 ngrok URL 添加到重定向 URI (例如 `https://<YOUR_NGROK_URL>/auth.html` ，) 。
>**注意**：MSAL 仅支持 OAuth 的隐式流。 请确保在 Azure 门户中启用应用程序中的隐式流 (默认情况下未启用它) 。 在 **"身份验证**"下，找到 **隐式授予** 部分并选择 **访问** 令牌和 ID 令牌 **的复选框**。 

## <a name="create-the-auth-popup-page"></a>创建身份验证弹出窗口页面

为了允许用户登录，你需要提供 Teams 应用将在弹出窗口中打开的 URL，以遵循身份验证流。 URL 需要位于域中，此页面需要执行的所有操作就是调用 `TeamsProvider.handleAuth()` 该方法。

您可以在 HTML 中为此添加一个新文件 (该文件应位于与) 相同的级别，并添加 `auth.html` `public` `index.html` 以下代码： 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a>添加组件

现在，你已准备好将任何 Microsoft Graph Toolkit组件添加到选项卡。 

您可以像平常一样将组件添加到 HTML 中。 例如，若要添加登录组件，将以下代码添加到以下正文 `index.html` 中：

```html
<mgt-login></mgt-login>
```

或者，可以将 JSX 中的组件添加到选项卡组件。 如果你使用 Microsoft Teams 应用扩展创建了 Teams 应用， `mgt-react` 我们建议Toolkit库。 若要了解更多信息，请参阅将 [Microsoft Graph Toolkit React](./use-toolkit-with-react.md)

首先，安装 `mgt-react` ：

```bash
npm install @microsoft/mgt-react
```

找到 `src/components/Tab.js` 该文件，然后从库导入想要使用 `mgt-react` 的组件。 例如，若要添加 `Login` 组件，请使用：

```js
import { Login } from "@microsoft/mgt-react"
```

然后，将组件添加到 `return()` 以下方法 `render()` 的语句 `Tab` 中：

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

若要测试应用程序，需要将应用程序上载到 Teams。 打开 Microsoft Teams 客户端，选择左侧菜单上的 **...，** 然后转到 **App Studio。** 单击清单 **编辑器** 选项卡，然后选择 **"导入现有应用"。**

找到项目目录， **将Development.zip** 文件上载到 **.publish** 文件夹内。

加载应用后，向下滚动到左侧菜单，然后选择"**测试和分发"。** 单击"**安装**"按钮，然后单击"**添加"。** 你将重定向到你创建的选项卡。

## <a name="next-steps"></a>后续步骤
- 请查看此有关生成 Teams 选项卡的 [分步教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)。
- 尝试在运动场 [中的组件](https://mgt.dev)。
- 在 Stack [Overflow](https://aka.ms/mgt-question)上提问。
- 在 GitHub 上报告 Bug 或保留 [功能请求](https://aka.ms/mgt)。