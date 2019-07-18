---
title: Microsoft Graph 工具包提供程序
description: Microsoft Graph 工具包提供程序为所有组件启用身份验证和 Microsoft Graph 访问。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 3e5d587e8c2690d2b71a2e70e41266519566f91e
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778710"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="285ff-103">Microsoft Graph 工具包提供程序</span><span class="sxs-lookup"><span data-stu-id="285ff-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="285ff-104">Microsoft Graph 工具包提供程序为所有组件启用身份验证和 Microsoft Graph 访问。</span><span class="sxs-lookup"><span data-stu-id="285ff-104">The Microsoft Graph Toolkit providers enable authentication and Microsoft Graph access for all components.</span></span> <span data-ttu-id="285ff-105">每个提供程序都提供用于获取调用 Microsoft Graph Api 所需的访问令牌的实现。</span><span class="sxs-lookup"><span data-stu-id="285ff-105">Each provider provides implementation for acquiring the necessary access token for calling the Microsoft Graph APIs.</span></span>

<span data-ttu-id="285ff-106">对于要使用提供程序的组件, 必须将该`Providers.globalProvider`属性设置为要使用的提供程序的值。</span><span class="sxs-lookup"><span data-stu-id="285ff-106">For the components to use a provider, you must set the `Providers.globalProvider` property to the value for a provider you'd like to use.</span></span>

<span data-ttu-id="285ff-107">下面的示例演示如何使用 MsalProvider。</span><span class="sxs-lookup"><span data-stu-id="285ff-107">The following example shows how to use the MsalProvider.</span></span>

```js
Providers.globalProvider = new MsalProvider({
  clientId: '[CLIENT_ID]'
});
```

<span data-ttu-id="285ff-108">此工具包实现以下提供程序:</span><span class="sxs-lookup"><span data-stu-id="285ff-108">The toolkit implements the following providers:</span></span>

- [<span data-ttu-id="285ff-109">MsalProvider</span><span class="sxs-lookup"><span data-stu-id="285ff-109">MsalProvider</span></span>](./providers/msal.md)
- [<span data-ttu-id="285ff-110">SharePointProvider</span><span class="sxs-lookup"><span data-stu-id="285ff-110">SharePointProvider</span></span>](./providers/sharepoint.md)
- [<span data-ttu-id="285ff-111">TeamsProvider</span><span class="sxs-lookup"><span data-stu-id="285ff-111">TeamsProvider</span></span>](./providers/teams.md)
- <span data-ttu-id="285ff-112">Office 外接程序提供程序 (即将推出)</span><span class="sxs-lookup"><span data-stu-id="285ff-112">Office Add-ins provider (coming soon)</span></span>

## <a name="get-started"></a><span data-ttu-id="285ff-113">入门</span><span class="sxs-lookup"><span data-stu-id="285ff-113">Get started</span></span>

<span data-ttu-id="285ff-114">您可以随时创建提供程序。</span><span class="sxs-lookup"><span data-stu-id="285ff-114">You can create a provider at any time.</span></span> <span data-ttu-id="285ff-115">我们建议您先创建提供程序, 然后再使用任何组件。</span><span class="sxs-lookup"><span data-stu-id="285ff-115">We recommend that you create the provider before you use any of the components.</span></span> <span data-ttu-id="285ff-116">本节介绍如何初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="285ff-116">This section describes how to initialize a provider.</span></span>

<span data-ttu-id="285ff-117">`Providers`全局变量公开以下属性和函数</span><span class="sxs-lookup"><span data-stu-id="285ff-117">The `Providers` global variable exposes the following properties and functions</span></span>

- `globalProvider : IProvider`

<span data-ttu-id="285ff-118">将此属性设置为要全局使用的提供程序。</span><span class="sxs-lookup"><span data-stu-id="285ff-118">Set this property to a provider that you want to use globally.</span></span> <span data-ttu-id="285ff-119">所有组件均使用此属性获取对提供程序的引用。</span><span class="sxs-lookup"><span data-stu-id="285ff-119">All components use this property to get a reference to the provider.</span></span> <span data-ttu-id="285ff-120">设置此属性将触发该`onProvidersChanged`事件。</span><span class="sxs-lookup"><span data-stu-id="285ff-120">Setting this property will fire the `onProvidersChanged` event.</span></span>

- `function onProviderUpdated(callbackFunction)`

<span data-ttu-id="285ff-121">当`callbackFunction`提供程序发生更改或提供程序的状态更改时, 将调用此函数。</span><span class="sxs-lookup"><span data-stu-id="285ff-121">The `callbackFunction` function will be called when a provider is changed or when the state of a provider changes.</span></span> <span data-ttu-id="285ff-122">`ProvidersChangedState`枚举值将传递给函数以指示更新的内容。</span><span class="sxs-lookup"><span data-stu-id="285ff-122">A `ProvidersChangedState` enum value will be passed to the function to indicate what updated.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="285ff-123">实现您自己的提供程序</span><span class="sxs-lookup"><span data-stu-id="285ff-123">Implement your own provider</span></span>

<span data-ttu-id="285ff-124">该工具包提供了两种创建新的提供程序的方法:</span><span class="sxs-lookup"><span data-stu-id="285ff-124">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="285ff-125">通过传入获取`SimpleProvider`访问令牌的函数来创建新的</span><span class="sxs-lookup"><span data-stu-id="285ff-125">Create a new `SimpleProvider` by passing in a function for getting an access token</span></span>
- <span data-ttu-id="285ff-126">扩展`IProvider`抽象类</span><span class="sxs-lookup"><span data-stu-id="285ff-126">Extend the `IProvider` abstract class</span></span>

<span data-ttu-id="285ff-127">有关详细信息, 请参阅[自定义提供程序](./providers/custom.md)文档中的每一个。</span><span class="sxs-lookup"><span data-stu-id="285ff-127">Read more about each one in the [custom providers](./providers/custom.md) documentation.</span></span>

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="285ff-128">对 Microsoft Graph 进行自己的调用</span><span class="sxs-lookup"><span data-stu-id="285ff-128">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="285ff-129">只要您初始化提供程序 (如上一节中所述), 所有组件都可以访问 Microsoft Graph, 而无需进行任何自定义。</span><span class="sxs-lookup"><span data-stu-id="285ff-129">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous section).</span></span> <span data-ttu-id="285ff-130">若要获取对组件使用的同一 Microsoft Graph SDK 的引用, 请首先获取对全局 IProvider 的引用, 然后使用该`Graph`对象, 如图所示。</span><span class="sxs-lookup"><span data-stu-id="285ff-130">To get a reference to the same Microsoft Graph SDK used by the components, first get a reference to the global IProvider and then use the `Graph` object, as shown.</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```

<span data-ttu-id="285ff-131">在某些情况下, 您可能需要传递其他权限, 具体取决于您要调用的 API。</span><span class="sxs-lookup"><span data-stu-id="285ff-131">There might be cases were you will need to pass additional permissions, depending on the API you're calling.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

<span data-ttu-id="285ff-132">该`graph`对象是[MICROSOFT graph Javascript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript)的一个实例, 可以使用它对 microsoft graph 进行任何调用。</span><span class="sxs-lookup"><span data-stu-id="285ff-132">The `graph` object is an instance of the [Microsoft Graph Javascript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) and you can use it to make any calls to Microsoft Graph.</span></span>
