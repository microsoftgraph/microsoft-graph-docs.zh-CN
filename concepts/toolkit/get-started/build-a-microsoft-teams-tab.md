---
title: 使用 Microsoft Graph 工具包生成 Microsoft 团队选项卡
description: 开始使用 Microsoft Graph 工具包生成 Microsoft 团队选项卡。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: c4ed3396d05c865fd483bc8b007cdc743c0e8419
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288537"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph 工具包生成 Microsoft 团队选项卡

本主题介绍如何在 Microsoft 团队解决方案中开始使用 Microsoft Graph 工具包。 入门涉及以下步骤：

1. 使用自定义选项卡创建新的团队应用程序。
2. 设置 ngrok 并创建隧道。
3. 添加 Microsoft Graph 工具包。
4. 初始化 Microsoft 团队提供程序。
5. 创建身份验证弹出页面。
6. 添加组件。
7. 测试您的应用程序。

## <a name="create-a-new-teams-application-with-a-custom-tab"></a>使用自定义选项卡创建新的团队应用程序

创建新的团队应用程序最简单的方法是将 [Microsoft 团队工具包扩展](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) 用于 Visual Studio Code。 按照说明 [设置新的团队项目](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project)。 进入 " **添加功能** " 屏幕时，依次选择 " **选项卡**" 和 " **个人" 选项卡**。

## <a name="set-up-ngrok-and-create-a-tunnel"></a>设置 ngrok 并创建隧道

为了稍后测试您的应用程序，您需要使用 HTTPS 以面向公众的 URL 托管应用程序。 使用以下命令安装 [ngrok](https://ngrok.com/download) 并创建从 Internet 到 localhost：3000的隧道：

```bash
ngrok http 3000
```
在项目目录中，找到 `.publish\Development.env` 文件并将值替换为 `baseUrl0` 您的 ngrok URL。

## <a name="add-the-microsoft-graph-toolkit"></a>添加 Microsoft Graph 工具包

您可以在应用程序中使用 Microsoft Graph 工具包，方法是通过 unpkg) 或安装 npm 程序包直接 (引用加载程序。 若要使用此工具包，你还需要 [Microsoft 团队 SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)。

### <a name="use-via-mgt-loader"></a>通过预加载加载程序使用
若要通过加载程序使用工具包和团队 SDK，请将以下引用添加到 `public/index.html` ：

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>通过 npm (ES6 模块使用) 
通过使用 ES6 模块中的工具包，可以完全控制捆绑过程，并允许您只捆绑应用程序所需的代码。 若要使用 ES6 模块，请将工具包和 Microsoft 团队 SDK 的 npm 包添加到项目中：

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a>初始化团队提供程序

Microsoft Graph 工具包提供程序启用对组件的 Microsoft Graph 的身份验证和访问。 若要了解详细信息，请参阅 [使用提供程序](../providers.md)。 [团队提供程序](../providers/teams.md)处理需要与团队 SDK 实现的所有逻辑和交互，以对用户进行身份验证。

您可以选择在 HTML 或 JavaScript 代码中初始化提供程序。 

### <a name="initialize-in-html"></a>在 HTML 中初始化

在中 `public/index.html` ，添加团队提供程序，如下所示。

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

将替换为您的 `<YOUR_CLIENT_ID>` 应用程序的客户端 ID 和 `<YOUR_NGROK_URL>` 您创建的 ngrok URL。

### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化

若要在 JavaScript 代码中初始化提供程序，请在 `src/components/App.js` 项目目录中找到该文件。 导入团队提供程序并初始化提供程序。

```js
import * as microsoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
将替换为 `<YOUR_CLIENT_ID>` 应用程序的客户端 ID。

### <a name="creating-an-appclient-id"></a>创建应用/客户端 ID
为了获取客户端 ID，需要在 Azure AD 中 [注册应用程序](../../auth-register-app-v2.md) 。 确保将 ngrok URL 的完整路径添加到 "重定向 Uri" 中的 "身份验证" 弹出页面 (例如， `https://<YOUR_NGROK_URL>/auth.html`) "。
>**注意**： MSAL 仅支持 OAuth 的隐式流。 请务必在 Azure 门户中的应用程序中启用隐式流， (默认情况下不启用它) 。 在 " **身份验证**" 下，找到 " **隐式授予** " 部分，然后选择 " **访问令牌** " 和 **ID 令牌**的复选框。 

## <a name="create-the-auth-popup-page"></a>创建身份验证弹出页面

若要允许用户登录，需要提供工作组应用将在弹出项中打开以遵循身份验证流的 URL。 URL 必须在您的域中，并且所有此页面都需要调用 `TeamsProvider.handleAuth()` 方法。

您可以在 HTML 中执行此操作，方法是在文件夹中添加一个新 `auth.html` 文件 `public` (该文件应与) 相同的级别 `index.html` ，并添加以下代码： 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a>添加组件

现在，你已准备好将任何 Microsoft Graph 工具包组件添加到你的选项卡。 

你可以像往常一样将组件添加到你的 HTML 中。 例如，若要添加登录组件，请将以下代码添加到的正文 `index.html` ：

```html
<mgt-login></mgt-login>
```

或者，可以将 JSX 中的组件添加到选项卡组件中。 `mgt-react`如果使用 Microsoft 团队工具包扩展创建了团队应用程序，我们建议使用库。 若要了解详细信息，请参阅将 [Microsoft Graph 工具包与响应结合使用](./use-toolkit-with-react.md#using-mgt-react)

首先，安装 `mgt-react` ：

```bash
npm install @microsoft/mgt-react
```

找到 `src/components/Tab.js` 文件，并从库中导入要使用的组件 `mgt-react` 。 例如，若要添加 `Login` 组件，请使用：

```js
import { Login } from "@microsoft/mgt-react"
```

然后，将该组件添加到的 `return()` 方法语句中 `render()` `Tab` ：

```jsx
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a>测试应用程序

使用以下命令生成和运行应用程序：
```bash
npm install
npm start
```

若要测试应用程序，需要将应用程序上载到团队。 打开 "Microsoft 团队客户端"，在左侧菜单中选择 " **...** "，然后转到 **应用程序 Studio**。 单击 " **清单编辑器** " 选项卡，然后选择 " **导入现有应用程序**"。

找到您的项目目录，并上传到 **. publish**文件夹中的**Development.zip**文件。

在应用程序加载后，向下滚动到左侧菜单，然后选择 " **测试和分发**"。 单击 " **安装** " 按钮，然后单击 " **添加**"。 你将被重定向到你创建的选项卡。

## <a name="next-steps"></a>后续步骤
- 请参阅本分步教程，了解如何 [生成团队选项卡](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)。
- 尝试 [样本](https://mgt.dev)中的组件。
- 在 [堆栈溢出](https://aka.ms/mgt-question)时提出问题。
- 在 [GitHub](https://aka.ms/mgt)上报告错误或保留功能请求。