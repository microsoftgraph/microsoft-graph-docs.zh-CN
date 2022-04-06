---
title: Microsoft Graph 工具包入门
description: 开始在应用程序中使用 Microsoft Graph 工具包。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 09e69c51e4cbb693f9923b793a80b687c0afbddc
ms.sourcegitcommit: 0249c86925c9b4797908394c952073b5d9137911
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2022
ms.locfileid: "64477676"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包入门

Microsoft Graph 工具包组件可以轻松添加到 Web 应用程序、SharePoint Web 部件或 Microsoft Teams 选项卡。 这些组件基于 Web 标准，可用于纯 JavaScript 项目或热门 Web 框架，如 Reach、Angular、Vue.js 等。

可以观看此简短视频，了解如何快速轻松地开始使用该工具包。

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

有关分步教程，请参阅 [Microsoft Graph Toolkit 模块入门](/learn/modules/msgraph-toolkit-intro/)。 

## <a name="set-up-your-microsoft-365-tenant"></a>设置 Microsoft 365 租户
若要使用工具包进行开发，需要访问 Microsoft 365 租户。 如果没有，可以在通过 [加入 Office 365 开发人员计划](https://developer.microsoft.com/microsoft-365/dev-program) 获取免费的 Office 365 开发人员订阅。 有关如何配置订阅的详细信息，请参阅 [设置 Microsoft 365 开发人员订阅](/office/developer-program/microsoft-365-developer-program-get-started)。

## <a name="set-up-your-development-environment"></a>设置开发环境
若要使用工具包进行开发，需要文本编辑器或 IDE。 可以使用所选的编辑器或 IDE，也可以免费安装和使用 [Visual Studio Code](https://code.visualstudio.com/download)。 还需要新式 Web 浏览器，如 Microsoft Edge、Google Chrome 或 Firefox。 还需要可从 [nodejs.org](https://nodejs.org) 安装的 Node.js 的 LTS 版本。

## <a name="using-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph 工具包
可以通过直接引用加载程序 (通过 unpkg) 或安装 npm 包，在应用程序中使用 Microsoft Graph 工具包。

# <a name="unpkg"></a>[unpkg](#tab/html)
若要通过 mgt-loader 使用工具包，请将脚本中的引用添加到代码中:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[npm](#tab/npm)
通过 ES6 模块使用工具包可以完全控制捆绑过程，并允许仅捆绑应用程序所需的代码。 若要使用 ES6 模块，请将 npm 包添加到项目中:

```cmd
npm install @microsoft/mgt
```
现在可以引用正在使用的页面中的所有组件:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a>NPM 包

Microsoft Graph 工具包由多个 NPM 包组成，仅允许包含应用程序所需的代码。

<b>@microsoft/mgt-element</b>

`@microsoft/mgt-element` 是仅包含用于生成组件和提供程序基类的核心包。 此包公开生成自己的组件所需的所有必需类和接口，并导出用于生成自定义提供程序的 [IProvider 接口和 SimpleProvider 类](../providers/custom.md)。

<b>@microsoft/mgt-components</b>

`@microsoft/mgt-components` 包包含所有 Microsoft Graph 连接的 Web 组件，例如 `Person`、`PeoplePicker` 等。 

**提供程序**

提供程序可通过单个包使用，并可根据需要进行安装。 以下提供程序包可用:

- <b>@microsoft/mgt-msal-provider</b>

    [`@microsoft/mgt-msal-provider`](../providers/msal.md) 包含 `MsalProvider` 和 `mgt-msal-provider` 组件。 MSAL 提供程序使用 msal.js 在 Web 应用和渐进式 Web 应用 (PWA) 中进行身份验证。

- <b>@microsoft/mgt-msal2-provider</b>

    [`@microsoft/mgt-msal2-provider`](../providers/msal2.md) 包含 `Msal2Provider` 和 `mgt-msal2-provider` 组件。 MSAL2 提供程序使用 msal-browser 在 Web 应用和 PWA 中进行身份验证。

-  <b>@microsoft/mgt-teams-provider</b>

    [`@microsoft/mgt-teams-provider`](../providers/teams.md) 包含 `TeamsProvider` 和 `mgt-teams-provider` 组件。 Microsoft Teams 提供程序在 Microsoft Teams 选项卡应用程序中启用身份验证。

-  <b>@microsoft/mgt-teams-msal2-provider</b>

    [`@microsoft/mgt-teams-msal2-provider`](../providers/teams.md) 包含 `TeamsMsal2Provider` 和 `mgt-teams-msal2-provider` 组件。 Microsoft Teams MSAL2 提供程序在 Microsoft Teams 选项卡应用程序中启用身份验证。

- <b>@microsoft/mgt-sharepoint-provider</b>

    [`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) 包含在 SharePoint 环境中进行身份验证的 `SharePointProvider`。 

- <b>@microsoft/mgt-proxy-provider</b>

    [`@microsoft/mgt-proxy-provider`](../providers/proxy.md) 包含通过后端服务代理 Graph 调用的应用程序的 `ProxyProvider`。 

<b>@microsoft/mgt</b>

 `@microsoft/mgt` 是包含上述所有包并将其导出的主包，所以可以通过单个包进行安装。 

<b>@microsoft/mgt-react</b>

[`@microsoft/mgt-react`](./mgt-react.md) 包包含所有自动生成的 React 组件，并依赖于 `@microsoft/mgt` 包。

<b>@microsoft/mgt-spfx</b>

[`@microsoft/mgt-spfx`](./mgt-spfx.md) 包包含在 SharePoint 框架解决方案中使用Microsoft Graph工具包所需的 SharePoint 框架库。

## <a name="next-steps"></a>后续步骤
现在可以开始使用 Microsoft Graph 工具包进行开发了! 以下指南可用于帮助你入门:

- [注册 Azure Active Directory 应用](./add-aad-app-registration.md)
- [生成 Web 应用 (JavaScript)](./build-a-web-app.md) (vanilla JavaScript)
- [构建 web 应用程序 (React)](./use-toolkit-with-react.md)
- [构建 web 应用 (Angular)](./use-toolkit-with-angular.md)
- [构建 SharePoint Web 部件](./build-a-sharepoint-web-part.md)
- [构建 Microsoft Teams 选项卡](./build-a-microsoft-teams-tab.md)
