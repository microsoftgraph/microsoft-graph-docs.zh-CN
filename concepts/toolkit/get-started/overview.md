---
title: Microsoft Graph Toolkit
description: 开始在应用程序中Graph Toolkit Microsoft 应用。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e84350a7835cac7914f5238110f74b3383047e13
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579590"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Microsoft Graph Toolkit

Microsoft Graph Toolkit组件可轻松添加到 Web 应用程序、SharePoint Web 部件或Microsoft Teams选项卡。 这些组件基于 Web 标准，可用于纯 JavaScript 项目或热门 Web 框架（如 Reach、Angular、Vue.js 等）。

你可以观看此简短视频，了解快速而轻松地开始使用 Toolkit。

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

有关分步教程，请参阅 Microsoft Graph Toolkit[入门模块](/learn/modules/msgraph-toolkit-intro/)。 

## <a name="set-up-your-microsoft-365-tenant"></a>设置 Microsoft 365 租户
为了使用租户进行Toolkit，你需要访问 Microsoft 365 租户。 如果你没有，可以通过加入开发人员计划Microsoft 365免费订阅Microsoft 365[订阅](https://developer.microsoft.com/microsoft-365/dev-program)。 若要详细了解如何配置订阅，请参阅设置Microsoft 365[开发人员订阅](/office/developer-program/microsoft-365-developer-program-get-started)。

## <a name="set-up-your-development-environment"></a>设置开发环境
若要使用 Toolkit 进行开发，您需要文本编辑器或 IDE。 可以使用自己选择的编辑器或 IDE，也可以免费[安装和Visual Studio Code](https://code.visualstudio.com/download) IDE。 你还需要新式 Web 浏览器，Microsoft Edge、Google Chrome 或 Firefox。 你还需要 LTS 版本的 Node.js，可以从 nodejs.org[安装。](https://nodejs.org)

## <a name="using-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph Toolkit
可以在应用程序中使用 Microsoft Graph Toolkit，方法为通过 unpkg (直接引用加载程序) 安装 npm 包。

# <a name="unpkg"></a>[unpkg](#tab/html)
若要通过 mgt-loader Toolkit脚本，请向代码添加脚本中的引用：

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[npm](#tab/npm)
通过 ES6 模块使用 Toolkit 可以完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。 若要使用 ES6 模块，请向项目添加 npm 包：

```cmd
npm install @microsoft/mgt
```
现在，你可以引用你正在使用的页面的所有组件：

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a>NPM 包

Microsoft Graph Toolkit由多个 NPM 包决定，从而仅包含应用程序所需的代码。

<b>@microsoft/mgt-element</b>

是仅包含用于生成组件和提供程序的基类 `@microsoft/mgt-element` 的核心程序包。 此包公开构建您自己的组件所需的所有必需类和接口，并导出用于生成自定义提供程序的 [IProvider 接口和 SimpleProvider](../providers/custom.md) 类。

<b>@microsoft/mgt-components</b>

程序包包含所有 Microsoft Graph连接的 Web 组件，如 、 `@microsoft/mgt-components` `Person` `PeoplePicker` 等。 

**提供程序**

提供程序可通过单个程序包提供，并可以根据需要进行安装。 以下提供程序包可用：

- <b>@micosoft/mgt-msal-provider</b>

    [`@micosoft/mgt-msal-provider`](../providers/msal.md) 包含 `MsalProvider` 和 `mgt-msal-provider` 组件。 MSAL 提供程序使用 msal.js 在 Web 应用中进行身份验证，使用渐进式 Web 应用 (PA) 。

- <b>@micosoft/mgt-msal2-provider</b>

    [`@micosoft/mgt-msal2-provider`](../providers/msal2.md) 包含 `Msal2Provider` 和 `mgt-msal2-provider` 组件。 MSAL 提供程序使用 msal-browser 在 Web 应用和 PWA 中进行身份验证。

-  <b>@microsoft/mgt-teams-provider</b>

    [`@microsoft/mgt-teams-provider`](../providers/teams.md) 包含 `TeamsProvider` 和 `mgt-teams-provider` 组件。 该Microsoft Teams在选项卡应用程序中Microsoft Teams身份验证。

- <b>@microsoft/mgt-sharepoint-provider</b>

    [`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md)包含 `SharePointProvider` 用于在环境中进行身份验证SharePoint。 

- <b>@microsoft/mgt-proxy-provider</b>

    [`@microsoft/mgt-proxy-provider`](../providers/proxy.md)包含 `ProxyProvider` 代理通过后端Graph调用的 for 应用程序。 

<b>@microsoft/mgt</b>

是包含上述所有程序包的主程序包，然后重新导出它们，以便可以通过你可以安装的单个程序包 `@microsoft/mgt` 获取它们。 

<b>@microsoft/mgt-react</b>

[`@microsoft/mgt-react`](./mgt-react.md)程序包包含所有自动生成的React组件，并依赖 `@microsoft/mgt` 该程序包。

<b>@microsoft/mgt-spfx</b>

[`@microsoft/mgt-spfx`](./mgt-spfx.md)该包包含SharePoint 框架解决方案中使用 Microsoft Graph Toolkit所需的SharePoint 框架库。

## <a name="polyfills"></a>Polyfills

如果使用的是 npm 包中的 ES6 模块，并且面向的浏览器（如 [IE11）](https://caniuse.com/#search=components) 在本机不支持 Web 组件，则需要在项目中包含填充，因为它们不会自动包含。 填充有助于填充仍在更新以支持 Web 组件标准的浏览器中缺少的浏览器功能。 有关说明和了解更多信息，请参阅 [填充文档](https://www.webcomponents.org/polyfills)。 

如果你通过 mgt-loader 脚本使用 Toolkit填充已包含在内。

## <a name="next-steps"></a>后续步骤
现在，你已准备好开始使用 Microsoft Graph Toolkit！ 以下指南可帮助你入门：

- [注册 Azure Active Directory 应用](./add-aad-app-registration.md)
- [使用 JavaScript (生成 ](./build-a-web-app.md) Web)  (javaScript) 
- [构建 web 应用程序 (React)](./use-toolkit-with-react.md)
- [构建 web 应用 (Angular)](./use-toolkit-with-angular.md)
- [构建 SharePoint Web 部件](./build-a-sharepoint-web-part.md)
- [构建 Microsoft Teams 选项卡](./build-a-microsoft-teams-tab.md)
