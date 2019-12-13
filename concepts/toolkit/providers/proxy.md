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
# <a name="proxy-provider"></a><span data-ttu-id="9eca1-103">代理提供程序</span><span class="sxs-lookup"><span data-stu-id="9eca1-103">Proxy provider</span></span>

<span data-ttu-id="9eca1-104">使用代理提供程序时，可以使用后端身份验证（如代表身份验证2.0）为 Microsoft Graph 工具包供电，方法是通过将所有呼叫通过您自己的后端路由到 Microsoft graph 工具包。</span><span class="sxs-lookup"><span data-stu-id="9eca1-104">When you use the proxy provider, you can use your backend authentication (such as Auth2.0 On-Behalf-Of flow) to power the Microsoft Graph Toolkit by routing all calls to Microsoft Graph through your own backend.</span></span>

<span data-ttu-id="9eca1-105">后端服务必须公开将为每个 Microsoft Graph 调用调用的 API。</span><span class="sxs-lookup"><span data-stu-id="9eca1-105">Your backend service must expose an API that will be called for every call to Microsoft Graph.</span></span> <span data-ttu-id="9eca1-106">例如，当组件尝试获取资源时，ProxyProvider 将改为调用基本 API 并追加该资源。</span><span class="sxs-lookup"><span data-stu-id="9eca1-106">For example, when a component attempts to get a resource, the ProxyProvider will instead call your base API and append that resource.</span></span>

<pre>https://graph.microsoft.com/v1.0/me => https://myurl.com/api/GraphProxy/v1.0/me</pre> 

<span data-ttu-id="9eca1-107">然后，您的 API 实现应代表用户调用 Microsoft Graph 并将结果返回到组件。</span><span class="sxs-lookup"><span data-stu-id="9eca1-107">Your API implementation should then call Microsoft Graph on behalf of the user and return the results to the component.</span></span>

<span data-ttu-id="9eca1-108">有关实现示例，请参阅[ASP.NET MVC 示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc)。</span><span class="sxs-lookup"><span data-stu-id="9eca1-108">For an implementation example, see the [ASP.NET MVC sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc).</span></span> 

<span data-ttu-id="9eca1-109">若要了解有关身份验证提供程序的详细信息，请参阅[提供程序](../providers.md)。</span><span class="sxs-lookup"><span data-stu-id="9eca1-109">To learn more about authentication providers, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="9eca1-110">入门</span><span class="sxs-lookup"><span data-stu-id="9eca1-110">Get started</span></span>

<span data-ttu-id="9eca1-111">您可以用 HTML 或 JavaScript 初始化代理提供程序。</span><span class="sxs-lookup"><span data-stu-id="9eca1-111">You can initialize the proxy provider in HTML or JavaScript.</span></span> <span data-ttu-id="9eca1-112">每页只应执行一次此操作。</span><span class="sxs-lookup"><span data-stu-id="9eca1-112">You should do this only once per page.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="9eca1-113">在 HTML 页面中初始化</span><span class="sxs-lookup"><span data-stu-id="9eca1-113">Initialize in your HTML page</span></span>

<span data-ttu-id="9eca1-114">在 HTML 中初始化代理提供程序是定义自定义服务器端身份验证的您自己的路由的最简单方法。</span><span class="sxs-lookup"><span data-stu-id="9eca1-114">Initializing the proxy provider in HTML is the simplest way to define your own route for custom server-side authentication.</span></span> <span data-ttu-id="9eca1-115">使用`mgt-proxy-provider`组件设置**graph-代理 url**。</span><span class="sxs-lookup"><span data-stu-id="9eca1-115">Use the `mgt-proxy-provider` component to set the **graph-proxy-url**.</span></span> <span data-ttu-id="9eca1-116">这会将定义的代理提供程序设置为全局提供程序。</span><span class="sxs-lookup"><span data-stu-id="9eca1-116">This will set the defined proxy provider as the global provider.</span></span>

```html
<mgt-proxy-provider graph-proxy-url="https://myurl.com/api/GraphProxy"></mgt-proxy-provider>
```

| <span data-ttu-id="9eca1-117">属性</span><span class="sxs-lookup"><span data-stu-id="9eca1-117">Attribute</span></span> | <span data-ttu-id="9eca1-118">说明</span><span class="sxs-lookup"><span data-stu-id="9eca1-118">Description</span></span> |
| --- | --- |
| <span data-ttu-id="9eca1-119">graph-代理-url</span><span class="sxs-lookup"><span data-stu-id="9eca1-119">graph-proxy-url</span></span>  | <span data-ttu-id="9eca1-120">代理 API 的基 URL。</span><span class="sxs-lookup"><span data-stu-id="9eca1-120">Base URL for the proxy API.</span></span> |


### <a name="initialize-in-javascript"></a><span data-ttu-id="9eca1-121">在 JavaScript 中初始化</span><span class="sxs-lookup"><span data-stu-id="9eca1-121">Initialize in JavaScript</span></span>

<span data-ttu-id="9eca1-122">您可以通过在 JavaScript 中初始化提供程序来提供更多选项。</span><span class="sxs-lookup"><span data-stu-id="9eca1-122">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy");
```

<span data-ttu-id="9eca1-123">（可选）通过将可选函数用作构造函数中的第二个参数，可以向代理 api 发送包含每个请求的其他标头。</span><span class="sxs-lookup"><span data-stu-id="9eca1-123">Optionally, you can send additional headers with each request to your proxy api by using an optional function as the second parameter in the constructor.</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy", async () => {
  return {
    header: 'value',
    header2: 'value2'
  };
);
```

<span data-ttu-id="9eca1-124">当您需要将令牌或其他标头传递给后端时，这将非常有用</span><span class="sxs-lookup"><span data-stu-id="9eca1-124">This is useful when you need to pass tokens or other headers to your backend</span></span>

<span data-ttu-id="9eca1-125">如果要使用`mgt-login`组件，还应为提供程序指定`login`和`logout`函数：</span><span class="sxs-lookup"><span data-stu-id="9eca1-125">If you will be using the `mgt-login` component, you should also specify the `login` and `logout` functions for the provider:</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

let provider = new ProxyProvider("https://myurl.com/api/GraphProxy");
provider.login = () => { /* will be called when "Sign In" is clicked */ };
provider.logout = () => { /* will be called when "Sign Out" is called */ };

Providers.globalProvider = provider;
```

