---
title: 使用 Microsoft Graph Toolkit
description: 开始使用 Microsoft Graph Toolkit 构建 Web Graph Toolkit。
ms.localizationpriority: medium
author: elisenyang
ms.openlocfilehash: 22f5e81f8c382694389ddcffbe5e0f8a77fa55a9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59103835"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph Toolkit

本主题介绍如何在用 vanilla JavaScript Graph Toolkit Web 应用程序中开始使用 Microsoft 应用程序。 有关分步教程，请尝试 Microsoft Graph Toolkit[入门。](/learn/modules/msgraph-toolkit-intro/) 若要了解如何将 web 应用与 web Toolkit，请参阅生成 Web 应用[ (React) 或生成](./use-toolkit-with-react.md)Web [ (Angular) 。 ](./use-toolkit-with-angular.md)

Microsoft Graph Toolkit入门包括以下步骤：
1. 将 Microsoft Graph Toolkit添加到你的项目中。
2. 初始化 MSAL2 提供程序。
3. 添加组件。
4. 测试应用程序。

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a>将 Microsoft Graph 工具包添加到项目
可以在应用程序中使用 Microsoft Graph Toolkit，方法为通过 unpkg (直接引用加载程序) 安装 npm 包。

# <a name="unpkg"></a>[unpkg](#tab/html)
若要通过 mgt-loader 使用 Toolkit，请向代码添加脚本中的引用：

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[npm](#tab/npm)
通过 ES6 模块使用 Toolkit 可完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。 若要使用 ES6 模块，请向项目添加 npm 包：

```cmd
npm install @microsoft/mgt
```

---

## <a name="initialize-the-msal2-provider"></a>初始化 MSAL2 提供程序
Microsoft Graph 工具包提供程序为组件启用身份验证和对 Microsoft Graph 的访问。 若要了解详细信息，请参阅[使用提供程序](../providers/providers.md)。 [MSAL2 提供程序](../providers/msal2.md)使用 msal-browser 登录用户并获取令牌。 可以在 HTML 或 JavaScript 中初始化此提供程序。

> **注意**：如果你当前正在使用 MSAL 提供程序，并且要更新到 MSAL2 提供程序，请按照此处列出的 [步骤操作](../providers/msal2.md#migrating-from-msal-provider-to-msal2-provider)。
如果要使用自己的后端身份验证，请使用代理 [提供程序](../providers/proxy.md) 替代 MSAL2 提供程序。

可以选择在 HTML 或 JavaScript 代码中初始化提供程序。 

# <a name="html"></a>[HTML](#tab/HTML)
将 `mgt-msal2-provider` 组件添加到 HTML 页面，将 设置为 `client-id` 应用程序 client-id。

```html
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
```
# <a name="javascript"></a>[JavaScript](#tab/JavaScript)
若要在 JavaScript 中初始化 MSAL 提供程序，请向应用程序添加以下代码：

```javascript
import { Providers, Msal2Provider } from '@microsoft/mgt';

Providers.globalProvider = new Msal2Provider({
  clientId: "<YOUR_CLIENT_ID>"
});
```

---

客户端 ID 是初始化提供程序所需的唯一属性，但您可以设置其他选项。 有关完整列表，请参阅[MSAL2 Provider。](../providers/msal2.md)

### <a name="creating-an-appclient-id"></a>创建应用/客户端 ID
若要获取客户端 ID，需要在 Azure AD 中 [注册](./add-aad-app-registration.md) 应用程序。

## <a name="add-components"></a>添加组件
初始化 MSAL2 提供程序后，可以开始使用任何Toolkit组件。

# <a name="html"></a>[HTML](#tab/HTML)
下面是使用 mgt-loader 的完整工作示例、HTML 中初始化的 MSAL2 提供程序和登录组件：

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

这是使用 ES6 模块、HTML 中初始化的 MSAL2 提供程序和登录组件的示例：

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

# <a name="javascript"></a>[JavaScript](#tab/JavaScript)
这是使用 ES6 模块、在 JavaScript 中初始化的 MSAL2 提供程序和登录组件的示例：

```javascript
import { Providers, Msal2Provider } from '@microsoft/mgt';

Providers.globalProvider = new Msal2Provider({
  clientId: "<YOUR_CLIENT_ID>"
});

function component() {
  const element = document.createElement('div');
  element.innerHTML = '<mgt-login></mgt-login>';
  return element;
}

document.body.appendChild(component());
```

---

## <a name="test-your-app"></a>测试应用

为了测试你的应用，MSAL 要求将页面托管在 Web 服务器中，以便进行身份验证重定向。 

如果刚开始操作并且想要玩游戏，可以在 Visual Studio Code或任何类似的轻型开发服务器中使用[Live](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) Server。 下载扩展名，然后使用实时服务器打开 HTML 文件。
> **注意：** 确保应用 **注册中的重定向 URI** 设置为托管应用程序的 localhost 端口。 转到 Azure 门户中的应用注册 [，](https://portal.azure.com)单击"管理"下的"身份验证"，然后添加正确的 **重定向 URI。**

## <a name="track-a-users-sign-in-state"></a>跟踪用户的登录状态

你可以检测用户何时成功登录，并相应地显示特定组件。 例如，如果用户已登录，则显示议程组件。 否则，显示登录界面。

若要正确检查用户的登录状态，使用 函数向 `providerUpdated` 事件添加事件 `Providers.onProviderUpdated` 处理程序。 在处理程序中，检查存储在 属性上的提供程序 `Providers.globalProvider.state` 状态。

# <a name="html"></a>[HTML](#tab/HTML)

如果使用的是 库 `mgt-loader` ，可以从全局 `Provider` `ProviderState` 属性访问 和 `mgt` 。

```html
<!DOCTYPE html>
<html>
<head>
  <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
</head>
<body>
  <mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
  <div id="main">
    <mgt-login></mgt-login>
  </div>
  <script>
    const loadAgenda = () => {
      if (mgt.Providers.globalProvider.state === mgt.ProviderState.SignedIn) {
        document.getElementById('main').innerHTML = '<mgt-agenda></mgt-agenda>';
      }
    }
    mgt.Providers.onProviderUpdated(loadAgenda);
  </script>
</body>
</html>
```

# <a name="javascript"></a>[JavaScript](#tab/JavaScript)

如果你通过 npm 包使用工具包，你可以从 导入 和 `Provider` `ProviderState` `@microsoft/mgt` 。

```javascript
import { Providers, ProviderState, Msal2Provider } from '@microsoft/mgt';

Providers.globalProvider = new Msal2Provider({
  clientId: "<YOUR_CLIENT_ID>"
});

const loadAgenda = () => {
  if (Providers.globalProvider.state === ProviderState.SignedIn) {
    document.getElementById('main').innerHTML = '<mgt-agenda></mgt-agenda>';
  }
};

Providers.onProviderUpdated(loadAgenda);
```

---

## <a name="next-steps"></a>后续步骤

- 请查看[Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/)入门教程。
- 在[样本](https://mgt.dev)中试用组件。
- 在 [Stack Overflow](https://aka.ms/mgt-question) 上提问。
- 在 [GitHub](https://aka.ms/mgt) 上报告 bug 或提出功能请求。
