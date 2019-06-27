---
title: 自定义提供程序
description: 如果您的应用程序中有现有的身份验证代码, 则创建自定义提供程序以启用 Microsoft Graph 工具包组件的身份验证和图形访问。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: acd96e6dc7e13b1e1fbfc5353e3db2132a23e246
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242969"
---
# <a name="custom-provider"></a><span data-ttu-id="28a93-103">自定义提供程序</span><span class="sxs-lookup"><span data-stu-id="28a93-103">Custom provider</span></span>

<span data-ttu-id="28a93-104">如果您的应用程序中有现有的身份验证代码, 则可以创建自定义提供程序, 以启用对 microsoft Graph 工具包组件的 Microsoft Graph 的身份验证和访问权限。</span><span class="sxs-lookup"><span data-stu-id="28a93-104">If you have existing authentication code in your application, you can create a custom provider to enable authentication and access to Microsoft Graph for Microsoft Graph Toolkit components.</span></span> <span data-ttu-id="28a93-105">有两种方法可以创建自定义提供程序:</span><span class="sxs-lookup"><span data-stu-id="28a93-105">There are two ways to create custom providers:</span></span>

- <span data-ttu-id="28a93-106">通过传入获取`SimpleProvider`访问令牌的函数来创建新的</span><span class="sxs-lookup"><span data-stu-id="28a93-106">Create a new `SimpleProvider` by passing in a function for getting an access token</span></span>
- <span data-ttu-id="28a93-107">扩展`IProvider`抽象类</span><span class="sxs-lookup"><span data-stu-id="28a93-107">Extend the `IProvider` abstract class</span></span>

<span data-ttu-id="28a93-108">本文更详细地介绍了每种方法。</span><span class="sxs-lookup"><span data-stu-id="28a93-108">This article describes each approach in more detail.</span></span>

## <a name="simpleprovider"></a><span data-ttu-id="28a93-109">SimpleProvider</span><span class="sxs-lookup"><span data-stu-id="28a93-109">SimpleProvider</span></span>

<span data-ttu-id="28a93-110">通过传入`SimpleProvider`将返回传入范围的访问令牌的函数来实例化类。</span><span class="sxs-lookup"><span data-stu-id="28a93-110">Instantiate the `SimpleProvider` class by passing in a function that will return an access token for passed-in scopes.</span></span>

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

<span data-ttu-id="28a93-111">此外, 还可以提供可从[登录](../components/login.md)组件`login`处理`logout`登录和注销调用的可选和函数。</span><span class="sxs-lookup"><span data-stu-id="28a93-111">In addition, you can also provide an optional `login` and `logout` functions that can handle the sign in and sign out calls from the [Login](../components/login.md) component.</span></span>

```ts
function getAccessToken(scopes: string[]) {
  // return a promise with accessToken string
}

function login() {
  // login code
}

function logout() {
  // logout code
}

let provider = new SimpleProvider(getAccessToken, login, logout);
```

### <a name="manage-state"></a><span data-ttu-id="28a93-112">管理状态</span><span class="sxs-lookup"><span data-stu-id="28a93-112">Manage state</span></span>

<span data-ttu-id="28a93-113">若要使组件了解提供程序的状态, 每当状态发生变化时, 都需要调用`provider.setState(state: ProviderState)`方法。</span><span class="sxs-lookup"><span data-stu-id="28a93-113">For the components to be aware of the state of the provider, you will need to call the `provider.setState(state: ProviderState)` method whenever the state changes.</span></span> <span data-ttu-id="28a93-114">例如, 当用户登录后, 请致电`provider.setState(ProviderState.SignedIn)`。</span><span class="sxs-lookup"><span data-stu-id="28a93-114">For example, when the user has signed in, call `provider.setState(ProviderState.SignedIn)`.</span></span> <span data-ttu-id="28a93-115">`ProviderState`枚举定义三种状态, 如下所示。</span><span class="sxs-lookup"><span data-stu-id="28a93-115">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a><span data-ttu-id="28a93-116">IProvider</span><span class="sxs-lookup"><span data-stu-id="28a93-116">IProvider</span></span>

<span data-ttu-id="28a93-117">您可以扩展`IProvider`抽象类以创建自己的提供程序。</span><span class="sxs-lookup"><span data-stu-id="28a93-117">You can extend the `IProvider` abstract class to create your own provider.</span></span>

### <a name="state"></a><span data-ttu-id="28a93-118">状态</span><span class="sxs-lookup"><span data-stu-id="28a93-118">State</span></span>

<span data-ttu-id="28a93-119">提供程序必须跟踪身份验证状态, 并在状态发生更改时更新组件。</span><span class="sxs-lookup"><span data-stu-id="28a93-119">A provider must keep track of the authentication state and update the components when the state changes.</span></span> <span data-ttu-id="28a93-120">`IProvider`类已实现`onStateChanged(eventHandler)`处理程序和`state: ProviderState`属性。</span><span class="sxs-lookup"><span data-stu-id="28a93-120">The `IProvider` class already implements the `onStateChanged(eventHandler)` handler and the `state: ProviderState` property.</span></span> <span data-ttu-id="28a93-121">您只需在实现中`setState(state:ProviderState)`使用方法来更新其更改时的状态。</span><span class="sxs-lookup"><span data-stu-id="28a93-121">You just need to use the `setState(state:ProviderState)` method in your implementation to update the state when it changes.</span></span> <span data-ttu-id="28a93-122">更新状态将触发`stateChanged`事件并自动更新所有组件。</span><span class="sxs-lookup"><span data-stu-id="28a93-122">Updating the state will fire the `stateChanged` event and update all the components automatically.</span></span>

### <a name="loginlogout"></a><span data-ttu-id="28a93-123">登录/注销</span><span class="sxs-lookup"><span data-stu-id="28a93-123">Login/Logout</span></span>

<span data-ttu-id="28a93-124">如果提供程序提供登录或注销功能, 请实现`login(): Promise<void>`和`logout(): Promise<void>`方法。</span><span class="sxs-lookup"><span data-stu-id="28a93-124">If your provider provides login or logout functionality, implement the `login(): Promise<void>` and `logout(): Promise<void>` methods.</span></span> <span data-ttu-id="28a93-125">这些方法是可选的。</span><span class="sxs-lookup"><span data-stu-id="28a93-125">These methods are optional.</span></span>

### <a name="access-token"></a><span data-ttu-id="28a93-126">访问令牌</span><span class="sxs-lookup"><span data-stu-id="28a93-126">Access token</span></span>

<span data-ttu-id="28a93-127">您必须实现`getAccessToken({'scopes': scopes[]}) : Promise<string>`方法。</span><span class="sxs-lookup"><span data-stu-id="28a93-127">You must implement the `getAccessToken({'scopes': scopes[]}) : Promise<string>` method.</span></span> <span data-ttu-id="28a93-128">此方法用于在每次调用 Microsoft Graph 之前获取有效令牌。</span><span class="sxs-lookup"><span data-stu-id="28a93-128">This method is used to get a valid token before every call to Microsoft Graph.</span></span>

### <a name="graph"></a><span data-ttu-id="28a93-129">流程图</span><span class="sxs-lookup"><span data-stu-id="28a93-129">Graph</span></span>

<span data-ttu-id="28a93-130">这些组件将 Microsoft Graph Javascript SDK 用于对 Microsoft Graph 的所有调用。</span><span class="sxs-lookup"><span data-stu-id="28a93-130">The components use the Microsoft Graph Javascript SDK for all calls to Microsoft Graph.</span></span> <span data-ttu-id="28a93-131">提供程序必须通过`graph`属性使 SDK 可用。</span><span class="sxs-lookup"><span data-stu-id="28a93-131">Your provider must make the SDK available through the `graph` property.</span></span> <span data-ttu-id="28a93-132">在构造函数中, 创建一个`Graph`新实例, 如下所示。</span><span class="sxs-lookup"><span data-stu-id="28a93-132">In your constructor, create a new `Graph` instance, as shown.</span></span>

```js
this.graph = new Graph(this);
```

<span data-ttu-id="28a93-133">`Graph`类是 MICROSOFT Graph SDK 顶部的光包装。</span><span class="sxs-lookup"><span data-stu-id="28a93-133">The `Graph` class is a light wrapper on top of the Microsoft Graph SDK.</span></span>

### <a name="example"></a><span data-ttu-id="28a93-134">示例</span><span class="sxs-lookup"><span data-stu-id="28a93-134">Example</span></span>

<span data-ttu-id="28a93-135">所有提供程序都扩展`IProvider`抽象类。</span><span class="sxs-lookup"><span data-stu-id="28a93-135">All the providers extend the `IProvider` abstract class.</span></span> <span data-ttu-id="28a93-136">有关示例, 请查看任何[现有提供程序](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/src/providers)的源代码。</span><span class="sxs-lookup"><span data-stu-id="28a93-136">For examples, take a look at the source code for any of the [existing providers](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/src/providers).</span></span>

## <a name="set-the-global-provider"></a><span data-ttu-id="28a93-137">设置全局提供程序</span><span class="sxs-lookup"><span data-stu-id="28a93-137">Set the global provider</span></span>

<span data-ttu-id="28a93-138">组件使用`Providers.globalProvider`属性访问提供程序。</span><span class="sxs-lookup"><span data-stu-id="28a93-138">Components use the `Providers.globalProvider` property to access a provider.</span></span> <span data-ttu-id="28a93-139">创建自己的提供程序后, 将此属性设置为提供程序。</span><span class="sxs-lookup"><span data-stu-id="28a93-139">After you create your own provider, set this property to your provider.</span></span>

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

<span data-ttu-id="28a93-140">所有组件都将收到新的提供程序, 并开始使用它。</span><span class="sxs-lookup"><span data-stu-id="28a93-140">All the components will be notified of the new provider and start using it.</span></span>
