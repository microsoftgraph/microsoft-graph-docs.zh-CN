---
title: 代理服务器提供商
description: 通过代理提供程序，你可以将自己的服务器端身份验证与 Microsoft Graph Toolkit。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c62718471c361cd9537bc8ee098c33e7b65830ec
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092251"
---
# <a name="proxy-provider"></a><span data-ttu-id="93cb0-103">代理服务器提供商</span><span class="sxs-lookup"><span data-stu-id="93cb0-103">Proxy provider</span></span>

<span data-ttu-id="93cb0-104">使用代理提供程序时，可以使用后端身份验证 (（如 Auth2.0 代表流) ）通过自己的后端路由对 Microsoft Graph 的所有调用来为 Microsoft Graph Toolkit 提供电源。</span><span class="sxs-lookup"><span data-stu-id="93cb0-104">When you use the proxy provider, you can use your backend authentication (such as Auth2.0 On-Behalf-Of flow) to power the Microsoft Graph Toolkit by routing all calls to Microsoft Graph through your own backend.</span></span>

<span data-ttu-id="93cb0-105">后端服务必须公开 API，该 API 将针对每次调用 Microsoft Graph 而调用。</span><span class="sxs-lookup"><span data-stu-id="93cb0-105">Your backend service must expose an API that will be called for every call to Microsoft Graph.</span></span> <span data-ttu-id="93cb0-106">例如，当组件尝试获取资源时，ProxyProvider 将改为调用基本 API 并追加该资源。</span><span class="sxs-lookup"><span data-stu-id="93cb0-106">For example, when a component attempts to get a resource, the ProxyProvider will instead call your base API and append that resource.</span></span>

<pre>https://graph.microsoft.com/v1.0/me => https://myurl.com/api/GraphProxy/v1.0/me</pre> 

<span data-ttu-id="93cb0-107">然后，API 实现应代表用户调用 Microsoft Graph，然后将结果返回到组件。</span><span class="sxs-lookup"><span data-stu-id="93cb0-107">Your API implementation should then call Microsoft Graph on behalf of the user and return the results to the component.</span></span>

<span data-ttu-id="93cb0-108">有关实现示例，请参阅 ASP.NET [MVC 示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc)。</span><span class="sxs-lookup"><span data-stu-id="93cb0-108">For an implementation example, see the [ASP.NET MVC sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc).</span></span> 

<span data-ttu-id="93cb0-109">若要了解有关身份验证提供程序的信息，请参阅 [提供程序](./providers.md)。</span><span class="sxs-lookup"><span data-stu-id="93cb0-109">To learn more about authentication providers, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="93cb0-110">开始行动</span><span class="sxs-lookup"><span data-stu-id="93cb0-110">Get started</span></span>

<span data-ttu-id="93cb0-111">可以使用 HTML 或 JavaScript 初始化代理提供程序。</span><span class="sxs-lookup"><span data-stu-id="93cb0-111">You can initialize the proxy provider in HTML or JavaScript.</span></span> <span data-ttu-id="93cb0-112">每页只能执行一次此操作。</span><span class="sxs-lookup"><span data-stu-id="93cb0-112">You should do this only once per page.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="93cb0-113">在 HTML 页中初始化</span><span class="sxs-lookup"><span data-stu-id="93cb0-113">Initialize in your HTML page</span></span>

<span data-ttu-id="93cb0-114">使用 HTML 初始化代理提供程序是定义您自己的自定义服务器端身份验证路由的最简单方法。</span><span class="sxs-lookup"><span data-stu-id="93cb0-114">Initializing the proxy provider in HTML is the simplest way to define your own route for custom server-side authentication.</span></span> <span data-ttu-id="93cb0-115">使用该 `mgt-proxy-provider` 组件设置 **graph-proxy-url。**</span><span class="sxs-lookup"><span data-stu-id="93cb0-115">Use the `mgt-proxy-provider` component to set the **graph-proxy-url**.</span></span> <span data-ttu-id="93cb0-116">这将将定义的代理提供程序设置为全局提供程序。</span><span class="sxs-lookup"><span data-stu-id="93cb0-116">This will set the defined proxy provider as the global provider.</span></span>

```html
<mgt-proxy-provider graph-proxy-url="https://myurl.com/api/GraphProxy"></mgt-proxy-provider>
```

| <span data-ttu-id="93cb0-117">属性</span><span class="sxs-lookup"><span data-stu-id="93cb0-117">Attribute</span></span> | <span data-ttu-id="93cb0-118">说明</span><span class="sxs-lookup"><span data-stu-id="93cb0-118">Description</span></span> |
| --- | --- |
| <span data-ttu-id="93cb0-119">graph-proxy-url</span><span class="sxs-lookup"><span data-stu-id="93cb0-119">graph-proxy-url</span></span>  | <span data-ttu-id="93cb0-120">代理 API 的基本 URL。</span><span class="sxs-lookup"><span data-stu-id="93cb0-120">Base URL for the proxy API.</span></span> |


### <a name="initialize-in-javascript"></a><span data-ttu-id="93cb0-121">在 JavaScript 中初始化</span><span class="sxs-lookup"><span data-stu-id="93cb0-121">Initialize in JavaScript</span></span>

<span data-ttu-id="93cb0-122">可以通过在 JavaScript 中初始化提供程序提供更多选项。</span><span class="sxs-lookup"><span data-stu-id="93cb0-122">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy");
```

<span data-ttu-id="93cb0-123">（可选）可以将可选函数用作构造函数中的第二个参数，将每个请求的其他标头发送到代理 API。</span><span class="sxs-lookup"><span data-stu-id="93cb0-123">Optionally, you can send additional headers with each request to your proxy api by using an optional function as the second parameter in the constructor.</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy", async () => {
  return {
    header: 'value',
    header2: 'value2'
  };
);
```

<span data-ttu-id="93cb0-124">当你需要将令牌或其他标头传递到后端时，这非常有用。</span><span class="sxs-lookup"><span data-stu-id="93cb0-124">This is useful when you need to pass tokens or other headers to your backend.</span></span>

<span data-ttu-id="93cb0-125">如果要使用该组件，还应为提供程序指定 `mgt-login` `login` and `logout` 函数：</span><span class="sxs-lookup"><span data-stu-id="93cb0-125">If you will be using the `mgt-login` component, you should also specify the `login` and `logout` functions for the provider:</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

let provider = new ProxyProvider("https://myurl.com/api/GraphProxy");
provider.login = () => { /* will be called when "Sign In" is clicked */ };
provider.logout = () => { /* will be called when "Sign Out" is called */ };

Providers.globalProvider = provider;
```

