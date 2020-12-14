---
title: 代理服务器提供商
description: 通过代理提供程序，你可以将自己的服务器端身份验证与 Microsoft Graph Toolkit。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: ab52ed5c1d3af2cb0dfb99e086245a5b33aa9908
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657883"
---
# <a name="proxy-provider"></a>代理服务器提供商

使用代理提供程序时，可以使用后端身份验证 (（如 Auth2.0 代表流) ）通过自己的后端路由对 Microsoft Graph 的所有调用来为 Microsoft Graph Toolkit 提供电源。

后端服务必须公开 API，该 API 将针对每次调用 Microsoft Graph 而调用。 例如，当组件尝试获取资源时，ProxyProvider 将改为调用基本 API 并追加该资源。

<pre>https://graph.microsoft.com/v1.0/me => https://myurl.com/api/GraphProxy/v1.0/me</pre> 

然后，API 实现应代表用户调用 Microsoft Graph，然后将结果返回到组件。

有关实现示例，请参阅 ASP.NET [MVC 示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc)。 

若要了解有关身份验证提供程序的信息，请参阅 [提供程序](./providers.md)。

## <a name="get-started"></a>入门

可以使用 HTML 或 JavaScript 初始化代理提供程序。 每页只能执行一次此操作。

### <a name="initialize-in-your-html-page"></a>在 HTML 页中初始化

使用 HTML 初始化代理提供程序是定义您自己的自定义服务器端身份验证路由的最简单方法。 使用该 `mgt-proxy-provider` 组件设置 **graph-proxy-url。** 这将将定义的代理提供程序设置为全局提供程序。

```html
<mgt-proxy-provider graph-proxy-url="https://myurl.com/api/GraphProxy"></mgt-proxy-provider>
```

| 属性 | 说明 |
| --- | --- |
| graph-proxy-url  | 代理 API 的基本 URL。 |


### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化

可以通过在 JavaScript 中初始化提供程序提供更多选项。

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy");
```

（可选）可以将可选函数用作构造函数中的第二个参数，通过每个请求向代理 api 发送其他标头。

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy", async () => {
  return {
    header: 'value',
    header2: 'value2'
  };
);
```

当你需要将令牌或其他标头传递到后端时，这非常有用

如果要使用该组件，还应为提供程序指定 `mgt-login` `login` and `logout` 函数：

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

let provider = new ProxyProvider("https://myurl.com/api/GraphProxy");
provider.login = () => { /* will be called when "Sign In" is clicked */ };
provider.logout = () => { /* will be called when "Sign Out" is called */ };

Providers.globalProvider = provider;
```

