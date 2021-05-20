---
title: Microsoft Graph Toolkit提供程序
description: Microsoft Graph Toolkit提供程序启用身份验证，并且 Microsoft Graph访问所有组件。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 05cbd59758b27266db7444333c72a2ba3a766ebb
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579695"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="466d9-103">Microsoft Graph Toolkit提供程序</span><span class="sxs-lookup"><span data-stu-id="466d9-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="466d9-104">Microsoft Graph Toolkit提供程序使应用程序能够使用 Microsoft 标识进行身份验证，并且只需几Graph几行代码Graph访问 Microsoft 标识。</span><span class="sxs-lookup"><span data-stu-id="466d9-104">The Microsoft Graph Toolkit providers enable your application to authenticate with Microsoft Identity and access Microsoft Graph in only few lines of code.</span></span> <span data-ttu-id="466d9-105">每个提供程序都处理用户身份验证并获取访问令牌以调用 Microsoft Graph API，因此，你不必自己编写此代码。</span><span class="sxs-lookup"><span data-stu-id="466d9-105">Each provider handles user authentication and acquiring the access tokens to call Microsoft Graph APIs, so that you don't have to write this code yourself.</span></span> 

<span data-ttu-id="466d9-106">你可以自行使用提供程序（无需组件）为应用快速实现身份验证，并调用 Microsoft Graph JavaScript 客户端 SDK。</span><span class="sxs-lookup"><span data-stu-id="466d9-106">You can use the providers on their own, without components, to quickly implement authentication for your app and make calls to Microsoft Graph via the JavaScript client SDK.</span></span>

<span data-ttu-id="466d9-107">使用 Microsoft Graph Toolkit组件时，提供程序是必需的，因为组件使用它们访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="466d9-107">The providers are required when using the Microsoft Graph Toolkit components as the components use them to access Microsoft Graph.</span></span> <span data-ttu-id="466d9-108">如果你已拥有自己的身份验证并且想要使用组件，可以改为使用 [自定义提供程序](./custom.md) 。</span><span class="sxs-lookup"><span data-stu-id="466d9-108">If you already have your own authentication and want to use the components, you can use a [custom provider](./custom.md) instead.</span></span>

<span data-ttu-id="466d9-109">该Toolkit包括以下提供程序。</span><span class="sxs-lookup"><span data-stu-id="466d9-109">The Toolkit includes the following providers.</span></span>

|<span data-ttu-id="466d9-110">提供程序</span><span class="sxs-lookup"><span data-stu-id="466d9-110">Providers</span></span>|<span data-ttu-id="466d9-111">说明</span><span class="sxs-lookup"><span data-stu-id="466d9-111">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="466d9-112">Msal</span><span class="sxs-lookup"><span data-stu-id="466d9-112">Msal</span></span>](./msal.md)|<span data-ttu-id="466d9-113">使用 MSAL.js 登录用户并获取与 Web 应用程序中的 Microsoft Graph一同使用的令牌。</span><span class="sxs-lookup"><span data-stu-id="466d9-113">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph in a web application.</span></span>|
|[<span data-ttu-id="466d9-114">Msal 2.0</span><span class="sxs-lookup"><span data-stu-id="466d9-114">Msal 2.0</span></span>](./msal2.md)| <span data-ttu-id="466d9-115">使用 msal-browser 登录用户并获取令牌，以便与 Web Graph Microsoft 应用程序一同使用。</span><span class="sxs-lookup"><span data-stu-id="466d9-115">Uses msal-browser to sign in users and acquire tokens to use with Microsoft Graph in a web application.</span></span> | 
|[<span data-ttu-id="466d9-116">百年</span><span class="sxs-lookup"><span data-stu-id="466d9-116">Electron</span></span>](./electron.md)|<span data-ttu-id="466d9-117">通过身份验证并提供 Microsoft Graph访问在一些应用内的组件。</span><span class="sxs-lookup"><span data-stu-id="466d9-117">Authenticates and provides Microsoft Graph access to components inside of Electron apps.</span></span>|
|[<span data-ttu-id="466d9-118">SharePoint</span><span class="sxs-lookup"><span data-stu-id="466d9-118">SharePoint</span></span>](./sharepoint.md)|<span data-ttu-id="466d9-119">通过身份验证并提供 Microsoft Graph访问 Web 部件内SharePoint权限。</span><span class="sxs-lookup"><span data-stu-id="466d9-119">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="466d9-120">Teams</span><span class="sxs-lookup"><span data-stu-id="466d9-120">Teams</span></span>](./teams.md)|<span data-ttu-id="466d9-121">通过身份验证并提供 Microsoft Graph访问选项卡内Microsoft Teams权限。</span><span class="sxs-lookup"><span data-stu-id="466d9-121">Authenticates and provides Microsoft Graph access to components inside  Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="466d9-122">代理</span><span class="sxs-lookup"><span data-stu-id="466d9-122">Proxy</span></span>](./proxy.md)|<span data-ttu-id="466d9-123">允许通过后端将所有调用路由到 Microsoft Graph后端身份验证。</span><span class="sxs-lookup"><span data-stu-id="466d9-123">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="466d9-124">自定义</span><span class="sxs-lookup"><span data-stu-id="466d9-124">Custom</span></span>](./custom.md)|<span data-ttu-id="466d9-125">创建自定义提供程序以使用应用程序的现有身份验证代码Graph访问 Microsoft 客户端。</span><span class="sxs-lookup"><span data-stu-id="466d9-125">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="initializing-a-provider"></a><span data-ttu-id="466d9-126">初始化提供程序</span><span class="sxs-lookup"><span data-stu-id="466d9-126">Initializing a provider</span></span>

<span data-ttu-id="466d9-127">若要在应用中使用提供程序，你需要初始化一个新提供程序，然后在 Providers 命名空间中将它设置为全局提供程序。</span><span class="sxs-lookup"><span data-stu-id="466d9-127">To use a provider in your app, you need to initialize a new provider and then set it as the global provider in the Providers namespace.</span></span> <span data-ttu-id="466d9-128">我们建议在开始使用任何组件之前执行此操作。</span><span class="sxs-lookup"><span data-stu-id="466d9-128">We recommend doing this before you start using any of the components.</span></span> <span data-ttu-id="466d9-129">可以通过两种方法之一执行此工作：</span><span class="sxs-lookup"><span data-stu-id="466d9-129">You can do this one of two ways:</span></span>

<span data-ttu-id="466d9-130">**选项 1：使用提供程序组件**</span><span class="sxs-lookup"><span data-stu-id="466d9-130">**Option 1: Use the provider component**</span></span>

<span data-ttu-id="466d9-131">可以直接在 HTML 中使用该提供程序的组件版本。</span><span class="sxs-lookup"><span data-stu-id="466d9-131">You can use the component version of the provider directly in your HTML.</span></span> <span data-ttu-id="466d9-132">在后台，将初始化新的提供程序并设置为全局提供程序。</span><span class="sxs-lookup"><span data-stu-id="466d9-132">Behind the scenes, a new provider is initialized and set as the global provider.</span></span> <span data-ttu-id="466d9-133">以下示例演示如何使用 Msal2Provider。</span><span class="sxs-lookup"><span data-stu-id="466d9-133">The following example shows how to use the Msal2Provider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="YOUR_CLIENT_ID"></mgt-msal2-provider>
```

<span data-ttu-id="466d9-134">**选项 2：在代码中初始化**</span><span class="sxs-lookup"><span data-stu-id="466d9-134">**Option 2: Initialize in code**</span></span>

<span data-ttu-id="466d9-135">通过 JavaScript 代码初始化提供程序，可以提供更多选项。</span><span class="sxs-lookup"><span data-stu-id="466d9-135">Initializing your provider in your JavaScript code enables you to provide more options.</span></span> <span data-ttu-id="466d9-136">为此，请创建一个新的提供程序实例，将属性的值设置为 `Providers.globalProvider` 希望使用的提供程序。</span><span class="sxs-lookup"><span data-stu-id="466d9-136">To do this, create a new provider instance and set the value of the `Providers.globalProvider` property to the provider you'd like to use.</span></span> <span data-ttu-id="466d9-137">以下示例演示如何使用 Msal2Provider。</span><span class="sxs-lookup"><span data-stu-id="466d9-137">The following example shows how to use the Msal2Provider.</span></span>

```js
import {Providers, Msal2Provider } from "@microsoft/mgt";
Providers.globalProvider = new Msal2Provider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> <span data-ttu-id="466d9-138">**注意：** 若要详细了解如何注册应用和获取客户端 ID，请参阅创建Azure Active Directory [应用](../get-started/add-aad-app-registration.md)。</span><span class="sxs-lookup"><span data-stu-id="466d9-138">**Note:** For details about how to register your app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>

## <a name="permission-scopes"></a><span data-ttu-id="466d9-139">权限范围</span><span class="sxs-lookup"><span data-stu-id="466d9-139">Permission Scopes</span></span>

<span data-ttu-id="466d9-140">建议在初始化提供程序时将应用程序需要的所有权限范围添加到属性或属性 (这不适用于 SharePoint `scopes` [提供程序](../providers/sharepoint.md)) 。</span><span class="sxs-lookup"><span data-stu-id="466d9-140">We recommend adding all the permission scopes your application needs to the `scopes` attribute or property when initializing your provider (this does not apply to the [SharePoint provider](../providers/sharepoint.md)).</span></span> <span data-ttu-id="466d9-141">这是可选的，但会通过向用户显示单个许可屏幕（即应用内所有组件请求的权限聚合列表）来改进用户体验，而不是显示每个组件的单独屏幕。</span><span class="sxs-lookup"><span data-stu-id="466d9-141">This is optional, but will improve your user experience by presenting a single consent screen to the user with an aggregated list of permissions requested by all components in your app, rather than presenting separate screens for each component.</span></span> <span data-ttu-id="466d9-142">以下示例显示如何使用 Msal2Provider 进行此操作。</span><span class="sxs-lookup"><span data-stu-id="466d9-142">The following examples show how to do this with the Msal2Provider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal2-provider>
```

<span data-ttu-id="466d9-143">如果要在代码中初始化提供程序，请提供 属性中数组中 `scopes` 的权限范围。</span><span class="sxs-lookup"><span data-stu-id="466d9-143">If you're initializing the provider in code, provide the permission scopes in an array in the `scopes` property.</span></span>

```js
import {Providers, Msal2Provider } from "@microsoft/mgt";
Providers.globalProvider = new Msal2Provider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

<span data-ttu-id="466d9-144">您可以在每个组件的文档页的 Microsoft Graph **权限** 部分找到每个组件所需的权限范围列表。</span><span class="sxs-lookup"><span data-stu-id="466d9-144">You can find the list of permission scopes required by each component in the **Microsoft Graph permissions** section of each component's documentation page.</span></span>

## <a name="provider-state"></a><span data-ttu-id="466d9-145">提供程序状态</span><span class="sxs-lookup"><span data-stu-id="466d9-145">Provider state</span></span>

<span data-ttu-id="466d9-146">提供程序跟踪用户的身份验证状态，并通知组件。</span><span class="sxs-lookup"><span data-stu-id="466d9-146">The provider keeps track of the user's authentication state and communicates it to the components.</span></span> <span data-ttu-id="466d9-147">例如，当用户成功登录时，将 更新为 ，向 组件发出信号，指示他们现在可以调用 `ProviderState` `SignedIn` Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="466d9-147">For example, when a user successfully signs in, the `ProviderState` is updated to `SignedIn`, signaling to the components that they are now able to make calls to Microsoft Graph.</span></span> <span data-ttu-id="466d9-148">枚举 `ProviderState` 定义三种状态，如下所示。</span><span class="sxs-lookup"><span data-stu-id="466d9-148">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

<span data-ttu-id="466d9-149">在某些情况下，你将希望显示某些功能或仅在用户成功登录后执行某个操作。</span><span class="sxs-lookup"><span data-stu-id="466d9-149">In some scenarios, you will want to show certain functionality or perform an action only after a user has successfully signed in.</span></span> <span data-ttu-id="466d9-150">可以访问和检查提供程序状态，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="466d9-150">You can access and check the provider state, as shown in the following example.</span></span>

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
<span data-ttu-id="466d9-151">您还可以使用 `Providers.onProviderUpdated` 方法在提供程序的状态发生更改时收到通知。</span><span class="sxs-lookup"><span data-stu-id="466d9-151">You can also use the `Providers.onProviderUpdated` method to get notified whenever the state of the provider changes.</span></span>

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

const providerStateChanged = () => {
  if (Providers.globalProvider.state === ProviderState.SignedIn) {
    // user is now signed in
  }
}

// register a callback for when the state changes
Providers.onProviderUpdated(providerStateChanged);

// remove callback if necessary
Providers.removeProviderUpdatedListener(providerStateChanged);
```

## <a name="getting-an-access-token"></a><span data-ttu-id="466d9-152">获取访问令牌</span><span class="sxs-lookup"><span data-stu-id="466d9-152">Getting an access token</span></span>

<span data-ttu-id="466d9-153">每个提供程序都公开一个称为 的函数，该函数可以检索当前访问令牌或检索提供的范围 `getAccessToken` 的新访问令牌。</span><span class="sxs-lookup"><span data-stu-id="466d9-153">Each provider exposes a function called `getAccessToken` that can retrieve the current access token or retrieve a new access token for the provided scopes.</span></span> <span data-ttu-id="466d9-154">以下示例演示如何获取具有权限范围的新访问 `User.Read` 令牌。</span><span class="sxs-lookup"><span data-stu-id="466d9-154">The following example shows how to get a new access token with the `User.Read` permission scope.</span></span>

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = await Providers.globalProvider.getAccessToken({scopes: ['User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="466d9-155">自行调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="466d9-155">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="466d9-156">所有组件都可以访问 Microsoft Graph，而无需任何自定义，只要初始化提供程序 (如前面的部分所述) 。</span><span class="sxs-lookup"><span data-stu-id="466d9-156">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous sections).</span></span> <span data-ttu-id="466d9-157">如果要自行调用 Microsoft Graph，可以通过获取对组件使用的同一 Microsoft Graph SDK 的引用来这样做。</span><span class="sxs-lookup"><span data-stu-id="466d9-157">If you want to make your own calls to Microsoft Graph, you can do so by getting a reference to the same Microsoft Graph SDK used by the components.</span></span> <span data-ttu-id="466d9-158">首先，获取对全局的引用 `IProvider` ，然后 `graph` 使用 对象，如下所示：</span><span class="sxs-lookup"><span data-stu-id="466d9-158">First, get a reference to the global `IProvider` and then use the `graph` object as shown:</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
<span data-ttu-id="466d9-159">在某些情况下，可能需要传递其他权限，具体取决于你调用的 API。</span><span class="sxs-lookup"><span data-stu-id="466d9-159">There might be cases where you need to pass additional permissions, depending on the API you're calling.</span></span> <span data-ttu-id="466d9-160">以下示例说明了具体的操作方法。</span><span class="sxs-lookup"><span data-stu-id="466d9-160">The following example shows how to do this.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a><span data-ttu-id="466d9-161">使用多个提供程序</span><span class="sxs-lookup"><span data-stu-id="466d9-161">Using multiple providers</span></span>

<span data-ttu-id="466d9-162">在某些情况下，应用程序将在不同的环境中运行，并且需要针对每个环境使用不同的提供程序。</span><span class="sxs-lookup"><span data-stu-id="466d9-162">In some scenarios, your application will run in different environments and require a different provider for each.</span></span> <span data-ttu-id="466d9-163">例如，应用可能同时作为 Web 应用程序和 Microsoft Teams 选项卡运行，这意味着你可能需要同时使用 Msal2Provider 和 TeamsProvider。</span><span class="sxs-lookup"><span data-stu-id="466d9-163">For example, the app might run as both a web application and a Microsoft Teams tab, which means you might need to use both the Msal2Provider and the TeamsProvider.</span></span> <span data-ttu-id="466d9-164">对于此方案，所有提供程序组件都有 用于创建回退链的属性， `depends-on` 如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="466d9-164">For this scenario, all provider components have the `depends-on` attribute to create a fallback chain, as shown in the following example.</span></span>

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal2-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal2-provider>
```

<span data-ttu-id="466d9-165">在此方案中，只有当你的应用作为 Web 应用程序运行并且 TeamsProvider 在当前环境中不可用时，才使用 Msal2Provider。</span><span class="sxs-lookup"><span data-stu-id="466d9-165">In this scenario, the Msal2Provider will only be used if your app is running as a web application and the TeamsProvider is not available in the current environment.</span></span>

<span data-ttu-id="466d9-166">若要在代码中完成相同的任务，可以在提供程序上使用 `isAvailable` 属性，如下所示。</span><span class="sxs-lookup"><span data-stu-id="466d9-166">To accomplish the same in code, you can use the `isAvailable` property on the provider, as shown.</span></span>

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new Msal2Provider(msalConfig)
}
```
## <a name="user-loginlogout"></a><span data-ttu-id="466d9-167">用户登录/注销</span><span class="sxs-lookup"><span data-stu-id="466d9-167">User Login/Logout</span></span>

<span data-ttu-id="466d9-168">为应用程序初始化正确的提供程序后，可以添加Toolkit[登录](../components/login.md)组件，以轻松快速地实现用户登录和注销。</span><span class="sxs-lookup"><span data-stu-id="466d9-168">When you have the right providers initialized for your application, you can add the Toolkit's [Login component](../components/login.md) to easily and quickly implement user login and logout.</span></span> <span data-ttu-id="466d9-169">该组件与提供程序一起处理所有身份验证逻辑和登录/注销功能。</span><span class="sxs-lookup"><span data-stu-id="466d9-169">The component works with the provider to handle all of the authentication logic and login/logout functionality.</span></span> <span data-ttu-id="466d9-170">以下示例使用 Msal2Provider 和 Login 组件。</span><span class="sxs-lookup"><span data-stu-id="466d9-170">The following example uses the Msal2Provider and the Login component.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="YOUR_CLIENT_ID"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="466d9-171">在需要自己实现此操作（而不是使用 Toolkit 的 Login 组件）的情况下，可以使用 提供程序的 和 方法来 `login` `logout` 实现此方案。</span><span class="sxs-lookup"><span data-stu-id="466d9-171">In scenarios where you want to implement this yourself, rather than using the Toolkit's Login component, you can do so by using the `login` and `logout` methods of the provider.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="466d9-172">实现你自己的提供程序</span><span class="sxs-lookup"><span data-stu-id="466d9-172">Implement your own provider</span></span>

<span data-ttu-id="466d9-173">在想要将 Toolkit 组件添加到具有预先存在的身份验证代码的应用程序的方案中，您可以创建一个连接到身份验证机制的自定义提供程序，而不是使用预定义的提供程序。</span><span class="sxs-lookup"><span data-stu-id="466d9-173">In scenarios where you want to add Toolkit components to an application with pre-existing authentication code, you can create a custom provider that hooks into your authentication mechanism, instead of using our predefined providers.</span></span> <span data-ttu-id="466d9-174">该工具包提供两种创建新提供程序的方法：</span><span class="sxs-lookup"><span data-stu-id="466d9-174">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="466d9-175">创建一 `SimpleProvider` 个通过传递函数从身份验证代码返回访问令牌的新建。</span><span class="sxs-lookup"><span data-stu-id="466d9-175">Create a new `SimpleProvider` that returns an access token from your authentication code by passing in a function.</span></span>
- <span data-ttu-id="466d9-176">扩展 `IProvider` 抽象类。</span><span class="sxs-lookup"><span data-stu-id="466d9-176">Extend the `IProvider` abstract class.</span></span>

<span data-ttu-id="466d9-177">有关每个提供程序的更多详细信息，请参阅 [自定义提供程序](../providers/custom.md)。</span><span class="sxs-lookup"><span data-stu-id="466d9-177">For more details about each one, see [custom providers](../providers/custom.md).</span></span>
