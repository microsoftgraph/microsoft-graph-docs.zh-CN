---
title: 代理提供程序
description: 代理提供程序允许您使用自己的服务器端身份验证和 Microsoft Graph 工具包。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 130811ded21013614c85cc90eea6f22c74e7cc73
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955769"
---
# <a name="proxy-provider"></a>代理提供程序

使用代理提供程序时，可以使用后端身份验证（如代表身份验证2.0）为 Microsoft Graph 工具包供电，方法是通过将所有呼叫通过您自己的后端路由到 Microsoft graph 工具包。

后端服务必须公开将为每个 Microsoft Graph 调用调用的 API。 例如，当组件尝试获取资源时，ProxyProvider 将改为调用基本 API 并追加该资源。

<pre>https://graph.microsoft.com/v1.0/me => https://myurl.com/api/GraphProxy/v1.0/me</pre> 

然后，您的 API 实现应代表用户调用 Microsoft Graph 并将结果返回到组件。

有关实现示例，请参阅[ASP.NET MVC 示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc)。 

若要了解有关身份验证提供程序的详细信息，请参阅[提供程序](../providers.md)。

## <a name="get-started"></a>入门

您可以用 HTML 或 JavaScript 初始化代理提供程序。 每页只应执行一次此操作。

### <a name="initialize-in-your-html-page"></a>在 HTML 页面中初始化

在 HTML 中初始化代理提供程序是定义自定义服务器端身份验证的您自己的路由的最简单方法。 使用`mgt-proxy-provider`组件设置**graph-代理 url**。 这会将定义的代理提供程序设置为全局提供程序。

```html
<mgt-proxy-provider graph-proxy-url="https://myurl.com/api/GraphProxy"></mgt-proxy-provider>
```

| 属性 | 说明 |
| --- | --- |
| graph-代理-url  | 代理 API 的基 URL。 |


### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化

您可以通过在 JavaScript 中初始化提供程序来提供更多选项。

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy");
```

（可选）通过将可选函数用作构造函数中的第二个参数，可以向代理 api 发送包含每个请求的其他标头。

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy", async () => {
  return {
    header: 'value',
    header2: 'value2'
  };
);
```

当您需要将令牌或其他标头传递给后端时，这将非常有用

如果要使用`mgt-login`组件，还应为提供程序指定`login`和`logout`函数：

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

let provider = new ProxyProvider("https://myurl.com/api/GraphProxy");
provider.login = () => { /* will be called when "Sign In" is clicked */ };
provider.logout = () => { /* will be called when "Sign Out" is called */ };

Providers.globalProvider = provider;
```

