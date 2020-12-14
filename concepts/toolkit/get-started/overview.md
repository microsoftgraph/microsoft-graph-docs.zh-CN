---
title: Getting started with the Microsoft Graph Toolkit
description: 开始在应用程序中Toolkit Microsoft Graph 应用。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: f1451213822e2489f04bb454c355125ed95b1aed
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664126"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Getting started with the Microsoft Graph Toolkit

Microsoft Graph Toolkit组件可轻松添加到 Web 应用程序、SharePoint Web 部件或 Microsoft Teams 选项卡。 这些组件基于 Web 标准，可用于纯 JavaScript 项目或热门 Web 框架（如 Reach、Angular、Vue.js等）。

你可以观看此简短视频，了解快速而轻松地开始使用 Toolkit。

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

## <a name="set-up-your-microsoft-365-tenant"></a>设置 Microsoft 365 租户
为了使用应用程序进行Toolkit，你需要访问 Microsoft 365 租户。 如果你没有，可以通过加入 Microsoft 365 开发人员计划获取 [免费的 Microsoft 365 开发人员订阅](https://developer.microsoft.com/microsoft-365/dev-program)。 若要详细了解如何配置订阅，请参阅 [设置 Microsoft 365 开发人员订阅](/office/developer-program/microsoft-365-developer-program-get-started)。

## <a name="set-up-your-development-environment"></a>设置开发环境
若要使用 Toolkit 进行开发，您需要文本编辑器或 IDE。 可以使用你选择的编辑器或 IDE，也可以免费安装和Visual Studio [代码](https://code.visualstudio.com/download) 。 你还需要一个新式 Web 浏览器，如 Microsoft Edge、Google Chrome 或 Firefox。 你还需要 LTS 版本的 Node.js，可以从[nodejs.org。](https://nodejs.org)

## <a name="using-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph Toolkit
可以在应用程序中使用 Microsoft Graph Toolkit，方法为直接通过取消 (加载程序) 安装 npm 包。

# <a name="unpkg"></a>[unpkg](#tab/html)
若要通过 mgt Toolkit使用脚本，请向代码添加脚本中的引用：

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[npm](#tab/npm)
通过 ES6 模块使用 Toolkit 可完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。 若要使用 ES6 模块，请向项目添加 npm 包：

```cmd
npm install @microsoft/mgt
```
现在，你可以引用你使用的页面的所有组件：

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a>NPM 包

Microsoft Graph Toolkit由多个 NPM 包决定，因此只需包含应用程序所需的代码。

<b>@microsoft/mgt-element</b>

它是仅包含用于生成组件和提供程序的基 `@microsoft/mgt-element` 类的核心包。 此包公开构建您自己的组件所需的所有必需类和接口，并导出用于生成自定义提供程序的 [IProvider 接口和 SimpleProvider](../providers/custom.md) 类。

<b>@microsoft/mgt 组件</b>

该 `@microsoft/mgt-components` 包包含所有 Microsoft Graph 连接的 Web 组件，如 `Person` ， `PeoplePicker` 等。 

**提供程序**

提供程序可通过单个程序包提供，并可以根据需要进行安装。 以下提供程序包可用：

- <b>@micosoft/mgt-msal-provider</b>

    [`@micosoft/mgt-msal-provider`](../providers/msal.md) 包含 `MsalProvider` 和 `mgt-msal-provider` 组件。 msal 提供程序利用msal.js Web 应用和 PWA 进行身份验证。

-  <b>@microsoft/mgt-teams-provider</b>

    [`@microsoft/mgt-teams-provider`](../providers/teams.md) 包含 `TeamsProvider` 和 `mgt-teams-provider` 组件。 Microsoft Teams 提供程序在 Microsoft Teams 选项卡应用程序中启用身份验证。

- <b>@microsoft/mgt-sharepoint-provider</b>

    [`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) 包含在 `SharePointProvider` SharePoint 环境中进行身份验证。 

- <b>@microsoft/mgt-proxy-provider</b>

    [`@microsoft/mgt-proxy-provider`](../providers/proxy.md) 包含 `ProxyProvider` 通过后端服务代理 Graph 调用的 for 应用程序。 

<b>@microsoft/mgt</b>

它是包含上述所有程序包的主程序包，并重新导出它们，以便它们可通过可安装的单个 `@microsoft/mgt` 程序包提供。 

<b>@microsoft/mgt-react</b>

该 [`@microsoft/mgt-react`](./mgt-react.md) 包包含所有自动生成的 React 组件，并依赖 `@microsoft/mgt` 该包。

## <a name="polyfills"></a>填充

如果使用的是 npm 包中的 ES6 模块，并且面向的浏览器（如 [IE11）](https://caniuse.com/#search=components) 本机不支持 Web 组件，则需要在项目中包含填充，因为它们不会自动包含在项目中。 填充有助于填充仍在更新以支持 Web 组件标准的浏览器中缺少的浏览器功能。 有关说明和了解更多信息，请参阅 [填充文档](https://www.webcomponents.org/polyfills)。 

如果通过 mgt-loader 脚本使用 Toolkit，则已包含填充。

## <a name="next-steps"></a>后续步骤
现在，你已准备好开始使用 Microsoft Graph Toolkit！ 以下指南可帮助你入门：

- [注册 Azure Active Directory 应用](./add-aad-app-registration.md)
- [使用 javaScript (javaScript)  (](./build-a-web-app.md) JavaScript) 
- [构建 web 应用程序 (React)](./use-toolkit-with-react.md)
- [构建 web 应用 (Angular)](./use-toolkit-with-angular.md)
- [构建 SharePoint Web 部件](./build-a-sharepoint-web-part.md)
- [构建 Microsoft Teams 选项卡](./build-a-microsoft-teams-tab.md)
