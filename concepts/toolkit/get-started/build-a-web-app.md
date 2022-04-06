---
title: 使用 Microsoft Graph Toolkit
description: 开始 Microsoft 网站生成 Web Graph Toolkit。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: e464f822f6c08c51443ac24b482c99081954acf7
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589007"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph Toolkit

本主题介绍如何在用 vanilla JavaScript 编写的 Web Graph Toolkit Microsoft 应用程序入门。 有关分步教程，请尝试开始 [Microsoft Graph Toolkit模块](/learn/modules/msgraph-toolkit-intro/)。 如果你想要了解如何将 web 应用程序与 web Toolkit，[请参阅生成 Web ](./use-toolkit-with-react.md) 应用 (React) 或生成 [Web (Angular) ](./use-toolkit-with-angular.md)。

Microsoft Graph Toolkit入门包括以下步骤：
1. 将 Microsoft Graph Toolkit添加到你的项目中。
2. 初始化 MSAL2 提供程序。
3. 添加组件。
4. 测试应用程序。

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a>将 Microsoft Graph 工具包添加到项目
可以通过直接引用加载程序 (通过 unpkg) 或安装 npm 包，在应用程序中使用 Microsoft Graph 工具包。

# <a name="unpkg"></a>[unpkg](#tab/html)
若要通过 mgt-loader 使用工具包，请将脚本中的引用添加到代码中:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[npm](#tab/npm)
通过 ES6 模块使用工具包可以完全控制捆绑过程，并允许仅捆绑应用程序所需的代码。 若要使用 ES6 模块，请将 npm 包添加到项目中:

```cmd
npm install @microsoft/mgt
```

---

## <a name="initialize-the-msal2-provider"></a>初始化 MSAL2 提供程序
Microsoft Graph 工具包提供程序为组件启用身份验证和对 Microsoft Graph 的访问。 若要了解详细信息，请参阅[使用提供程序](../providers/providers.md)。 [MSAL2 提供程序](../providers/msal2.md)使用 msal-browser 登录用户并获取令牌。 可以在 HTML 或 JavaScript 中初始化此提供程序。

> **注意**：如果当前使用的是 MSAL 提供程序，并且要更新到 MSAL2 提供程序，请按照此处列出的 [步骤操作](../providers/msal2.md#migrating-from-msal-provider-to-msal2-provider)。
如果要使用自己的后端身份验证，请使用代理 [提供程序](../providers/proxy.md) 替代 MSAL2 提供程序。

可以选择在 HTML 或 JavaScript 代码中初始化提供程序。 

# <a name="html"></a>[HTML](#tab/HTML)
将组件 `mgt-msal2-provider` 添加到 HTML 页面，将 设置为 `client-id` 应用程序 client-id。

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

客户端 ID 是初始化提供程序所需的唯一属性，但您可以设置其他选项。 有关完整列表，请参阅 [MSAL2 提供程序](../providers/msal2.md)。

### <a name="creating-an-appclient-id"></a>创建应用/客户端 ID
若要获取客户端 ID，需要在客户端 ID 中[注册](./add-aad-app-registration.md)Azure AD。

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

如果刚开始操作并且想要玩游戏，可以在 Visual Studio Code或任何类似的轻型开发服务器中使用 [Live](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) Server。 下载扩展名，然后使用实时服务器打开 HTML 文件。
> **注意：** 确保应用 **注册中的重定向 URI** 设置为托管应用程序的 localhost 端口。 转到应用中的应用注册Azure 门户"管理 [](https://portal.azure.com)"下的"身份验证"，然后添加正确的 **重定向 URI**。

## <a name="track-a-users-sign-in-state"></a>跟踪用户的登录状态

你可以检测用户何时成功登录，并相应地显示特定组件。 例如，如果用户已登录，则显示议程组件。 否则，显示登录界面。

若要正确检查用户的登录状态，使用 函数向 `providerUpdated` 事件添加事件 `Providers.onProviderUpdated` 处理程序。 在处理程序中，检查存储在 属性上的提供程序 `Providers.globalProvider.state` 状态。

# <a name="html"></a>[HTML](#tab/HTML)

如果使用的是 库`mgt-loader`，可以从全局`Provider``ProviderState`属性访问 和 `mgt` 。

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

如果你通过 npm 包使用工具包，你可以从 导入 `Provider` 和 `ProviderState` `@microsoft/mgt`。

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

- 请查看 Microsoft [开始 microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/)分步教程。
- 在[样本](https://mgt.dev)中试用组件。
- 在 [Stack Overflow](https://aka.ms/mgt-question) 上提问。
- 在 [GitHub](https://aka.ms/mgt) 上报告 bug 或提出功能请求。
