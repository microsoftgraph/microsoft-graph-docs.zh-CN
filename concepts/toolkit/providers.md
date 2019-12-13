---
title: Microsoft Graph 工具包提供程序
description: Microsoft Graph 工具包提供程序为所有组件启用身份验证和 Microsoft Graph 访问。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 221258b49d9a5217829633c7882b9dd4f9d2a221
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955783"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="38520-103">Microsoft Graph 工具包提供程序</span><span class="sxs-lookup"><span data-stu-id="38520-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="38520-104">Microsoft Graph 工具包提供程序为所有组件启用身份验证和 Microsoft Graph 访问。</span><span class="sxs-lookup"><span data-stu-id="38520-104">The Microsoft Graph Toolkit providers enable authentication and Microsoft Graph access for all components.</span></span> <span data-ttu-id="38520-105">每个提供程序都提供用于获取调用 Microsoft Graph Api 所需的访问令牌的实现。</span><span class="sxs-lookup"><span data-stu-id="38520-105">Each provider provides implementation for acquiring the necessary access token for calling the Microsoft Graph APIs.</span></span>

<span data-ttu-id="38520-106">对于要使用提供程序的组件，必须将该`Providers.globalProvider`属性设置为要使用的提供程序的值。</span><span class="sxs-lookup"><span data-stu-id="38520-106">For the components to use a provider, you must set the `Providers.globalProvider` property to the value for a provider you'd like to use.</span></span>

<span data-ttu-id="38520-107">下面的示例演示如何使用 MsalProvider。</span><span class="sxs-lookup"><span data-stu-id="38520-107">The following example shows how to use the MsalProvider.</span></span>

```js
Providers.globalProvider = new MsalProvider({
  clientId: '[CLIENT_ID]'
});
```

<span data-ttu-id="38520-108">此工具包实现以下提供程序：</span><span class="sxs-lookup"><span data-stu-id="38520-108">The toolkit implements the following providers:</span></span>

- [<span data-ttu-id="38520-109">MsalProvider</span><span class="sxs-lookup"><span data-stu-id="38520-109">MsalProvider</span></span>](./providers/msal.md)
- [<span data-ttu-id="38520-110">SharePointProvider</span><span class="sxs-lookup"><span data-stu-id="38520-110">SharePointProvider</span></span>](./providers/sharepoint.md)
- [<span data-ttu-id="38520-111">TeamsProvider</span><span class="sxs-lookup"><span data-stu-id="38520-111">TeamsProvider</span></span>](./providers/teams.md)
- [<span data-ttu-id="38520-112">ProxyProvider</span><span class="sxs-lookup"><span data-stu-id="38520-112">ProxyProvider</span></span>](./providers/proxy.md)
- [<span data-ttu-id="38520-113">SimpleProvider</span><span class="sxs-lookup"><span data-stu-id="38520-113">SimpleProvider</span></span>](./providers/custom.md)

<span data-ttu-id="38520-114">您可以随时创建提供程序。</span><span class="sxs-lookup"><span data-stu-id="38520-114">You can create a provider at any time.</span></span> <span data-ttu-id="38520-115">我们建议您先创建提供程序，然后再使用任何组件。</span><span class="sxs-lookup"><span data-stu-id="38520-115">We recommend that you create the provider before you use any of the components.</span></span> <span data-ttu-id="38520-116">本节介绍如何初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="38520-116">This section describes how to initialize a provider.</span></span>

## <a name="providers-namespace"></a><span data-ttu-id="38520-117">提供程序命名空间</span><span class="sxs-lookup"><span data-stu-id="38520-117">Providers namespace</span></span>

<span data-ttu-id="38520-118">`Providers`命名空间公开以下属性和函数：</span><span class="sxs-lookup"><span data-stu-id="38520-118">The `Providers` namespace exposes the following properties and functions:</span></span>

- `globalProvider : IProvider`

<span data-ttu-id="38520-119">将此属性设置为要全局使用的提供程序。</span><span class="sxs-lookup"><span data-stu-id="38520-119">Set this property to a provider that you want to use globally.</span></span> <span data-ttu-id="38520-120">所有组件均使用此属性获取对提供程序的引用。</span><span class="sxs-lookup"><span data-stu-id="38520-120">All components use this property to get a reference to the provider.</span></span> <span data-ttu-id="38520-121">设置此属性将触发该`onProvidersChanged`事件。</span><span class="sxs-lookup"><span data-stu-id="38520-121">Setting this property will fire the `onProvidersChanged` event.</span></span>

- `function onProviderUpdated(callbackFunction)`

<span data-ttu-id="38520-122">当`callbackFunction`提供程序发生更改或提供程序的状态更改时，将调用此函数。</span><span class="sxs-lookup"><span data-stu-id="38520-122">The `callbackFunction` function will be called when a provider is changed or when the state of a provider changes.</span></span> <span data-ttu-id="38520-123">`ProvidersChangedState`枚举值将传递给函数以指示更新的内容。</span><span class="sxs-lookup"><span data-stu-id="38520-123">A `ProvidersChangedState` enum value will be passed to the function to indicate what updated.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="38520-124">实现您自己的提供程序</span><span class="sxs-lookup"><span data-stu-id="38520-124">Implement your own provider</span></span>

<span data-ttu-id="38520-125">该工具包提供了两种创建新的提供程序的方法：</span><span class="sxs-lookup"><span data-stu-id="38520-125">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="38520-126">通过传入获取`SimpleProvider`访问令牌的函数来创建新的。</span><span class="sxs-lookup"><span data-stu-id="38520-126">Create a new `SimpleProvider` by passing in a function for getting an access token.</span></span>
- <span data-ttu-id="38520-127">扩展`IProvider`抽象类。</span><span class="sxs-lookup"><span data-stu-id="38520-127">Extend the `IProvider` abstract class.</span></span>

<span data-ttu-id="38520-128">有关每个的详细信息，请参阅[自定义提供程序](./providers/custom.md)。</span><span class="sxs-lookup"><span data-stu-id="38520-128">For more details about each one, see [custom providers](./providers/custom.md).</span></span>

## <a name="using-multiple-providers"></a><span data-ttu-id="38520-129">使用多个提供程序</span><span class="sxs-lookup"><span data-stu-id="38520-129">Using multiple providers</span></span>

<span data-ttu-id="38520-130">在某些情况下，您的应用程序将在不同的环境中运行，并需要不同的提供程序。</span><span class="sxs-lookup"><span data-stu-id="38520-130">In some scenarios, your application will run in a different environment and require a different provider.</span></span> <span data-ttu-id="38520-131">例如，应用程序可能同时作为 web 应用程序和 Microsoft 团队选项卡运行，您可能需要使用 MsalProvider 和 TeamsProvider。</span><span class="sxs-lookup"><span data-stu-id="38520-131">For example, the app might run as both a web application and a Microsoft Teams tab and you might need to use the MsalProvider and the TeamsProvider.</span></span> <span data-ttu-id="38520-132">对于此方案，所有提供程序组件都`depends-on`具有创建回退链的属性，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="38520-132">For this scenario, all provider components have the `depends-on` attribute to create a fallback chain, as shown in the following example.</span></span>

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

<span data-ttu-id="38520-133">在这种情况下，仅当 TeamsProvider 在当前环境中不可用时，才会使用 MsalProvider。</span><span class="sxs-lookup"><span data-stu-id="38520-133">In this scenario, the MsalProvider will only be used if the TeamsProvider is not available in the current environment.</span></span>

<span data-ttu-id="38520-134">若要在代码中实现相同，可以使用提供`isAvailable`程序上的属性，如下所示。</span><span class="sxs-lookup"><span data-stu-id="38520-134">To accomplish the same in code, you can use the `isAvailable` property on the provider, as shown.</span></span>

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="38520-135">对 Microsoft Graph 进行自己的调用</span><span class="sxs-lookup"><span data-stu-id="38520-135">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="38520-136">只要您初始化提供程序（如上一节中所述），所有组件都可以访问 Microsoft Graph，而无需进行任何自定义。</span><span class="sxs-lookup"><span data-stu-id="38520-136">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous section).</span></span> <span data-ttu-id="38520-137">若要获取对组件使用的同一 Microsoft Graph SDK 的引用，请首先获取对全局 IProvider 的引用，然后使用该`Graph`对象，如下所示：</span><span class="sxs-lookup"><span data-stu-id="38520-137">To get a reference to the same Microsoft Graph SDK used by the components, first get a reference to the global IProvider and then use the `Graph` object, as shown:</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```

<span data-ttu-id="38520-138">在某些情况下，您可能需要传递其他权限，具体取决于您要调用的 API。</span><span class="sxs-lookup"><span data-stu-id="38520-138">There might be cases were you will need to pass additional permissions, depending on the API you're calling.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

<span data-ttu-id="38520-139">该`graph`对象是[MICROSOFT graph Javascript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript)的一个实例，可以使用它对 microsoft graph 进行任何调用。</span><span class="sxs-lookup"><span data-stu-id="38520-139">The `graph` object is an instance of the [Microsoft Graph Javascript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) and you can use it to make any calls to Microsoft Graph.</span></span>
