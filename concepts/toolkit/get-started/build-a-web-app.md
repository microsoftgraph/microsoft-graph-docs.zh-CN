---
title: 使用 Microsoft Graph 应用程序生成 web Toolkit
description: 开始使用 Microsoft Graph 应用程序生成 web Toolkit。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 974f6351bdce985089d93f607210c8eb47b902ba
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961350"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph 应用程序生成 web Toolkit

本主题介绍如何在用 vanilla JavaScript Toolkit Web 应用程序中开始使用 Microsoft Graph 应用程序。 有关分步教程，请尝试 Microsoft Graph Toolkit[入门。](/learn/modules/msgraph-toolkit-intro/) 如果你想要了解如何将 Toolkit 与 Web 框架一同使用，请参阅生成 Web 应用 [ (React) ](./use-toolkit-with-react.md) 或 使用 Angular (生成 web [) ](./use-toolkit-with-angular.md)。

Microsoft Graph Toolkit入门包括以下步骤：
1. 将 Microsoft Graph Toolkit添加到你的项目中。
2. 初始化 MSAL 提供程序。
3. 添加组件。
4. 测试应用程序。

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a>将 Microsoft Graph Toolkit添加到你的项目
可以在应用程序中使用 Microsoft Graph Toolkit，方法为通过 unpkg (直接引用加载程序) 安装 npm 包。

# <a name="unpkg"></a>[unpkg](#tab/html)
若要通过 mgt-loader Toolkit脚本，请向代码添加脚本中的引用：

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[npm](#tab/npm)
通过 ES6 模块Toolkit可完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。 若要使用 ES6 模块，请向项目添加 npm 包：

```cmd
npm install @microsoft/mgt
```

---


> **注意**：如果你面向的浏览器（如 IE11）在本机不支持 Web 组件，可能需要包含 [填充](./overview.md#polyfills)。

## <a name="initialize-the-msal-provider"></a>初始化 MSAL 提供程序
Microsoft Graph Toolkit提供程序支持对组件的 Microsoft Graph 进行身份验证和访问。 若要了解更多信息，请参阅 [使用提供程序](../providers/providers.md)。 [MSAL 提供程序](../providers/msal.md)MSAL.js登录用户并获取令牌。 可以在 HTML 或 JavaScript 中初始化 MSAL 提供程序。

如果要使用自己的后端身份验证，请使用代理 [提供程序](../providers/proxy.md) 替代 MSAL 提供程序。

可以选择在 HTML 或 JavaScript 代码中初始化提供程序。 

# <a name="html"></a>[html](#tab/HTML)
将 `mgt-msal-provider` 组件添加到 HTML 页面，将 设置为 `client-id` 应用程序 client-id。

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
# <a name="js"></a>[js](#tab/JavaScript)
若要在 JavaScript 中初始化 MSAL 提供程序，请向应用程序添加以下代码：

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


客户端 ID 是初始化提供程序所需的唯一属性，但您可以设置其他选项。 有关完整列表，请参阅[Msal Provider。](../providers/msal.md)

### <a name="creating-an-appclient-id"></a>创建应用/客户端 ID
若要获取客户端 ID，需要在 Azure AD 中 [注册](./add-aad-app-registration.md) 应用程序。 
>**注意**：MSAL 仅支持 OAuth 的隐式流。 请确保在 Azure 门户应用程序中启用隐式流 (默认情况下不会启用它) 。 在 **身份验证** 下，找到 **隐式授予** 部分，并选中 **访问** 令牌和 **ID 令牌的复选框**。 

## <a name="add-components"></a>添加组件
初始化 MSAL 提供程序后，可以开始使用任何Toolkit组件。

# <a name="html"></a>[html](#tab/HTML)
下面是使用 mgt-loader 的完整工作示例、HTML 中初始化的 MSAL 提供程序和登录组件：

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

这是使用 ES6 模块、HTML 中初始化的 MSAL 提供程序和 Login 组件的示例：

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[js](#tab/JavaScript)
这是使用 ES6 模块、在 JavaScript 中初始化的 MSAL 提供程序和登录组件的示例：

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})

function component() {
    const element = document.createElement('div');
    element.innerHTML = '<mgt-login></mgt-login>'
    return element;
}

document.body.appendChild((component()));
```

---


## <a name="test-your-app"></a>测试应用

为了测试你的应用，MSAL 要求将页面托管在 Web 服务器中，以便进行身份验证重定向。 

如果你刚开始工作并且想要玩游戏，可以在 Visual Studio 代码或任何类似的轻型开发服务器中使用 [Live](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) Server。 下载扩展名，然后使用实时服务器打开 HTML 文件。 
> **注意：** 确保应用 **注册中的重定向 URI** 设置为托管应用程序的 localhost 端口。 转到 Azure 门户中的应用注册 [，](https://portal.azure.com)单击"管理"下的"身份验证"，然后添加正确的 **重定向 URI。**

## <a name="next-steps"></a>后续步骤
- 请查看 Microsoft [Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) 入门教程。
- 尝试在运动场中的 [组件](https://mgt.dev)。
- 在 Stack [Overflow 上提问](https://aka.ms/mgt-question)。
- 在 GitHub 上报告 Bug 或保留 [功能请求](https://aka.ms/mgt)。
