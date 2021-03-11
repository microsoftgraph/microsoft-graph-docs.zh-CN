---
title: 使用 Microsoft Graph 工具生成 Microsoft Teams Toolkit
description: 开始使用 Microsoft Graph Toolkit 构建 Microsoft Teams 选项卡。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 757c7eb8a94b0f6936a21f5ecb6f126cde36b6ad
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721563"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph 工具生成 Microsoft Teams Toolkit

本主题介绍如何在 Microsoft Teams 解决方案中开始使用 Microsoft Graph Toolkit。 入门包括以下步骤：

1. 使用自定义选项卡创建新的 Teams 应用程序。
2. 设置 ngrok 并创建隧道。
3. 添加 Microsoft Graph Toolkit。
4. 初始化 Microsoft Teams 提供程序。
5. 创建身份验证弹出页。
6. 添加组件。
7. 测试你的应用。

## <a name="create-a-new-teams-application-with-a-custom-tab"></a>使用自定义选项卡创建新的 Teams 应用程序

创建新 Teams 应用的最简单方法是使用 [Microsoft Teams](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) Toolkit扩展Visual Studio Code。 按照说明 [设置新的 Teams 项目](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project)。 当你进入"添加 **功能** "屏幕时，选择 **"选项卡**"，然后选择" **个人"选项卡**。

## <a name="set-up-ngrok-and-create-a-tunnel"></a>设置 ngrok 并创建隧道

为了稍后测试应用程序，您需要使用 HTTPS 通过面向公众的 URL 承载应用程序。 通过 [以下命令安装 ngrok，](https://ngrok.com/download) 并创建从 Internet 到 localhost：3000 的隧道：

```bash
ngrok http 3000
```
在项目目录中，找到 `.publish\Development.env` 该文件，并将其值替换为 `baseUrl0` ngrok URL。

## <a name="add-the-microsoft-graph-toolkit"></a>添加 Microsoft Graph Toolkit

可以在应用程序中使用 Microsoft Graph Toolkit，方法为通过 unpkg (或安装 npm 包) 加载程序。 若要使用Toolkit，你还需要[Microsoft Teams SDK。](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)

### <a name="use-via-mgt-loader"></a>通过 mgt-loader 使用
若要通过Toolkit使用 Toolkit 和 Teams SDK，请添加以下引用 `public/index.html` ：

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>通过 npm (ES6 模块) 
使用Toolkit ES6 模块进行绑定将让你完全控制捆绑过程，并允许你仅捆绑应用程序所需的代码。 若要使用 ES6 模块，请为项目添加 Toolkit 和 Microsoft Teams SDK 的 npm 包：

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a>初始化 Teams 提供程序

Microsoft Graph Toolkit提供程序支持对组件的 Microsoft Graph 进行身份验证和访问。 若要了解更多信息，请参阅["使用提供程序"。](../providers/providers.md) [Teams 提供程序](../providers/teams.md)处理需要通过 Teams SDK 实现以对用户进行身份验证的所有逻辑和交互。

你可以选择在 HTML 或 JavaScript 代码中初始化提供程序。 

### <a name="initialize-in-html"></a>在 HTML 中初始化

In `public/index.html` ， add the Teams provider as shown.

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

用 `<YOUR_CLIENT_ID>` 应用程序的客户端 ID 和 `<YOUR_NGROK_URL>` 您创建的 ngrok URL 替换。

### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化

若要在 JavaScript 代码中初始化提供程序，请在项目 `src/components/App.js` 目录中找到该文件。 导入 Teams 提供商并初始化提供商。

```js
import * as microsoftTeams from "@microsoft/teams-js";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
替换为 `<YOUR_CLIENT_ID>` 应用程序的客户端 ID。

### <a name="creating-an-appclient-id"></a>创建应用/客户端 ID
若要获取客户端 ID，需要在 Azure AD [中注册应用程序](../../auth-register-app-v2.md) 。 请确保将您的 ngrok URL 与身份验证弹出窗口页面的完整路径添加到重定向 URI (例如 `https://<YOUR_NGROK_URL>/auth.html` ，) 。
>**注意**：MSAL 仅支持 OAuth 的隐式流。 请确保在 Azure 门户中启用应用程序中的隐式流 (默认情况下不会启用它) 。 在 **"身份验证**"下，找到 **隐式授予** 部分，并选中 **访问** 令牌和 **ID 令牌的复选框**。 

## <a name="create-the-auth-popup-page"></a>创建身份验证弹出页

为了允许用户登录，你需要提供 Teams 应用将在弹出窗口中打开的 URL，以遵循身份验证流。 URL 需要位于域中，此页面需要执行的所有操作就是调用 `TeamsProvider.handleAuth()` 该方法。

您可以通过在文件夹文件夹中添加新文件来在 HTML 中 (该文件应处于与) 相同的级别，并添加 `auth.html` `public` `index.html` 以下代码： 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a>添加组件

现在，你已准备好将任何 Microsoft Graph Toolkit组件添加到你的选项卡。 

您可以像正常操作一样将组件添加到 HTML。 例如，若要添加登录组件，请向以下代码的正文添加 `index.html` ：

```html
<mgt-login></mgt-login>
```

或者，可以将 JSX 中的组件添加到 Tab 组件。 如果你使用 Microsoft Teams 应用扩展创建了 Teams 应用， `mgt-react` 我们建议Toolkit库。 若要了解更多信息，请参阅 [将 Microsoft Graph Toolkit React](./use-toolkit-with-react.md)

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

使用以下命令生成并运行应用程序：
```bash
npm install
npm start
```

若要测试应用程序，需要将应用程序上载到 Teams。 打开 Microsoft Teams 客户端，选择左侧菜单上的 **...，** 然后转到 **App Studio。** 单击清单 **编辑器** 选项卡，然后选择 **"导入现有应用"。**

找到项目目录，Development.zip **.publish****文件夹内** 上传文件。

加载应用后，向下滚动左侧菜单，然后选择"**测试和分发"。** 单击 **"安装**"按钮，然后单击"**添加"。** 您将重定向到您创建的选项卡。

## <a name="next-steps"></a>后续步骤
- 请查看此有关生成 Teams 选项卡的 [分步教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)。
- 尝试在运动场 [中的组件](https://mgt.dev)。
- 在 Stack [Overflow](https://aka.ms/mgt-question)上提问。
- 报告 Bug 或在 GitHub 上保留 [功能请求](https://aka.ms/mgt)。
