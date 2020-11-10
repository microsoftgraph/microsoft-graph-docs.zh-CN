---
title: Microsoft Graph 工具包入门
description: 开始在应用程序中使用 Microsoft Graph 工具包。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e3739bb6180e19569ae40e873d3a018bbb541833
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977133"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包入门

可以轻松地将 Microsoft Graph 工具包组件添加到 web 应用程序、SharePoint web 部件或 Microsoft 团队选项卡。 这些组件基于 web 标准，可在普通 JavaScript 项目中使用，也可用于常见的 web 框架，如 "接触"、"角度"、"Vue.js" 等。

您可以观看这段短视频，了解如何快速轻松地开始使用工具包。

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

## <a name="set-up-your-microsoft-365-tenant"></a>设置你的 Microsoft 365 租户
若要使用工具包进行开发，您需要访问 Microsoft 365 租户。 如果没有，则可以通过 [加入 microsoft 365 开发人员计划](https://developer.microsoft.com/microsoft-365/dev-program)来获取免费的 microsoft 365 开发人员订阅。 有关如何配置订阅的详细信息，请参阅 [Set up a Microsoft 365 developer 订阅](/office/developer-program/microsoft-365-developer-program-get-started)。

## <a name="set-up-your-development-environment"></a>设置开发环境
若要使用工具包进行开发，您将需要文本编辑器或 IDE。 您可以使用您选择的编辑器或 IDE，也可以免费安装和使用 [Visual Studio Code](https://code.visualstudio.com/download) 。 你还需要一个新式 web 浏览器，如 Microsoft Edge、Google Chrome 或 Firefox。 您还需要 Node.js 的 LTS 版本，可以从 [nodejs.org](https://nodejs.org)安装。

## <a name="using-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph 工具包
您可以在应用程序中使用 Microsoft Graph 工具包，方法是通过 unpkg) 或安装 npm 程序包直接 (引用加载程序。

### <a name="use-via-mgt-loader"></a>通过预加载加载程序使用
若要通过预加载程序使用该工具包，请将脚本中的引用添加到代码中：

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>通过 npm (ES6 模块使用) 
通过使用 ES6 模块中的工具包，可以完全控制捆绑过程，并允许您只捆绑应用程序所需的代码。 若要使用 ES6 模块，请将 npm 包添加到项目中：

```bash
npm install @microsoft/mgt
```
现在，您可以引用要使用的页面中的所有组件：

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

或者，只引用所需的组件，避免加载其他所有内容：
```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

#### <a name="polyfills"></a>Polyfills.ts

如果您使用 npm 程序包中的 ES6 模块，并且您针对的是不是本机支持 web 组件的 [浏览器（如 IE11](https://caniuse.com/#search=components) ），则需要在项目中包含 polyfills.ts，因为它们不会自动包含在内。 Polyfills.ts 帮助您在浏览器中填写缺少的浏览器功能，这些功能仍处于更新以支持 webcComponent 标准的过程中。 有关说明并了解详细信息，请参阅 [polyfills.ts 文档](https://www.webcomponents.org/polyfills)。 

如果使用的是 "polyfills.ts"，则可通过 "预加载加载程序" 脚本使用该工具包。

## <a name="next-steps"></a>后续步骤
现在，你可以开始使用 Microsoft Graph 工具包进行开发了！ 以下指南可帮助您入门：

- [创建 Azure Active Directory 应用程序](./add-aad-app-registration.md)
- [构建 web 应用程序](./build-a-web-app.md) (vanilla JavaScript) 
- [构建 SharePoint Web 部件](./build-a-sharepoint-web-part.md)
- [构建 Microsoft Teams 选项卡](./build-a-microsoft-teams-tab.md)
- [将此工具包与响应结合使用](./use-toolkit-with-react.md)
- [使用具有角度的工具包](./use-toolkit-with-angular.md)
