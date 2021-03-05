---
title: Microsoft Graph Toolkit提供程序
description: Microsoft Graph Toolkit提供程序支持所有组件的身份验证和 Microsoft Graph 访问。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c6fa59632464d0cfa801b07a30d6a5cf94ae5c76
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470282"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="13ac0-103">Microsoft Graph Toolkit提供程序</span><span class="sxs-lookup"><span data-stu-id="13ac0-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="13ac0-104">Microsoft Graph Toolkit提供程序使应用程序能够使用 Microsoft Identity 进行身份验证，并且只需几行代码访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="13ac0-104">The Microsoft Graph Toolkit providers enable your application to authenticate with Microsoft Identity and access Microsoft Graph in only few lines of code.</span></span> <span data-ttu-id="13ac0-105">每个提供程序都处理用户身份验证并获取访问令牌以调用 Microsoft Graph API，这样你不必自己编写此代码。</span><span class="sxs-lookup"><span data-stu-id="13ac0-105">Each provider handles user authentication and acquiring the access tokens to call Microsoft Graph APIs, so that you don't have to write this code yourself.</span></span> 

<span data-ttu-id="13ac0-106">你可以自行使用提供程序，而无需使用组件，以快速实现应用的身份验证，并可以通过 JavaScript 客户端 SDK 调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="13ac0-106">You can use the providers on their own, without components, to quickly implement authentication for your app and make calls to Microsoft Graph via the JavaScript client SDK.</span></span>

<span data-ttu-id="13ac0-107">使用 Microsoft Graph Toolkit组件时，提供程序是必需的，因为组件使用它们来访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="13ac0-107">The providers are required when using the Microsoft Graph Toolkit components as the components use them to access Microsoft Graph.</span></span> <span data-ttu-id="13ac0-108">如果你已拥有自己的身份验证并且想要使用组件，可以改为使用 [自定义](./custom.md) 提供程序。</span><span class="sxs-lookup"><span data-stu-id="13ac0-108">If you already have your own authentication and want to use the components, you can use a [custom provider](./custom.md) instead.</span></span>

<span data-ttu-id="13ac0-109">该Toolkit包括以下提供程序。</span><span class="sxs-lookup"><span data-stu-id="13ac0-109">The Toolkit includes the following providers.</span></span>

|<span data-ttu-id="13ac0-110">提供程序</span><span class="sxs-lookup"><span data-stu-id="13ac0-110">Providers</span></span>|<span data-ttu-id="13ac0-111">说明</span><span class="sxs-lookup"><span data-stu-id="13ac0-111">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="13ac0-112">Msal</span><span class="sxs-lookup"><span data-stu-id="13ac0-112">Msal</span></span>](./msal.md)|<span data-ttu-id="13ac0-113">使用MSAL.js登录用户并获取令牌以在 Web 应用程序中与 Microsoft Graph 一同使用。</span><span class="sxs-lookup"><span data-stu-id="13ac0-113">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph in a web application.</span></span>|
|[<span data-ttu-id="13ac0-114">都云</span><span class="sxs-lookup"><span data-stu-id="13ac0-114">Electron</span></span>](./electron.md)|<span data-ttu-id="13ac0-115">验证并提供对"一线"应用内组件的 Microsoft Graph 访问。</span><span class="sxs-lookup"><span data-stu-id="13ac0-115">Authenticates and provides Microsoft Graph access to components inside of Electron apps.</span></span>|
|[<span data-ttu-id="13ac0-116">SharePoint</span><span class="sxs-lookup"><span data-stu-id="13ac0-116">SharePoint</span></span>](./sharepoint.md)|<span data-ttu-id="13ac0-117">对 SharePoint Web 部件内的组件进行身份验证并提供 Microsoft Graph 访问。</span><span class="sxs-lookup"><span data-stu-id="13ac0-117">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="13ac0-118">Teams</span><span class="sxs-lookup"><span data-stu-id="13ac0-118">Teams</span></span>](./teams.md)|<span data-ttu-id="13ac0-119">对 Microsoft Teams 选项卡内的组件进行身份验证并提供 Microsoft Graph 访问权限。</span><span class="sxs-lookup"><span data-stu-id="13ac0-119">Authenticates and provides Microsoft Graph access to components inside  Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="13ac0-120">代理</span><span class="sxs-lookup"><span data-stu-id="13ac0-120">Proxy</span></span>](./proxy.md)|<span data-ttu-id="13ac0-121">允许通过后端路由对 Microsoft Graph 的所有调用来使用后端身份验证。</span><span class="sxs-lookup"><span data-stu-id="13ac0-121">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="13ac0-122">自定义</span><span class="sxs-lookup"><span data-stu-id="13ac0-122">Custom</span></span>](./custom.md)|<span data-ttu-id="13ac0-123">创建自定义提供程序以使用应用程序的现有身份验证代码启用身份验证并访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="13ac0-123">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="initializing-a-provider"></a><span data-ttu-id="13ac0-124">初始化提供程序</span><span class="sxs-lookup"><span data-stu-id="13ac0-124">Initializing a provider</span></span>

<span data-ttu-id="13ac0-125">若要在应用中使用提供程序，需要初始化新提供程序，然后在提供程序命名空间中将提供程序设置为全局提供程序。</span><span class="sxs-lookup"><span data-stu-id="13ac0-125">To use a provider in your app, you need to initialize a new provider and then set it as the global provider in the Providers namespace.</span></span> <span data-ttu-id="13ac0-126">建议在开始使用任何组件之前执行此操作。</span><span class="sxs-lookup"><span data-stu-id="13ac0-126">We recommend doing this before you start using any of the components.</span></span> <span data-ttu-id="13ac0-127">可以通过两种方法之一执行此操作：</span><span class="sxs-lookup"><span data-stu-id="13ac0-127">You can do this one of two ways:</span></span>

<span data-ttu-id="13ac0-128">**选项 1：使用提供程序组件**</span><span class="sxs-lookup"><span data-stu-id="13ac0-128">**Option 1: Use the provider component**</span></span>

<span data-ttu-id="13ac0-129">可以直接在 HTML 中使用该提供程序的组件版本。</span><span class="sxs-lookup"><span data-stu-id="13ac0-129">You can use the component version of the provider directly in your HTML.</span></span> <span data-ttu-id="13ac0-130">在后台，将初始化新提供程序并设置为全局提供程序。</span><span class="sxs-lookup"><span data-stu-id="13ac0-130">Behind the scenes, a new provider is initialized and set as the global provider.</span></span> <span data-ttu-id="13ac0-131">以下示例演示如何使用 MsalProvider。</span><span class="sxs-lookup"><span data-stu-id="13ac0-131">The following example shows how to use the MsalProvider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

<span data-ttu-id="13ac0-132">**选项 2：在代码中初始化**</span><span class="sxs-lookup"><span data-stu-id="13ac0-132">**Option 2: Initialize in code**</span></span>

<span data-ttu-id="13ac0-133">在 JavaScript 代码中初始化提供程序使您能够提供更多选项。</span><span class="sxs-lookup"><span data-stu-id="13ac0-133">Initializing your provider in your JavaScript code enables you to provide more options.</span></span> <span data-ttu-id="13ac0-134">为此，请创建新的提供程序实例，将属性的值设置为要 `Providers.globalProvider` 使用的提供程序。</span><span class="sxs-lookup"><span data-stu-id="13ac0-134">To do this, create a new provider instance and set the value of the `Providers.globalProvider` property to the provider you'd like to use.</span></span> <span data-ttu-id="13ac0-135">以下示例演示如何使用 MsalProvider。</span><span class="sxs-lookup"><span data-stu-id="13ac0-135">The following example shows how to use the MsalProvider.</span></span>

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> <span data-ttu-id="13ac0-136">**注意：** 若要详细了解如何注册应用和获取客户端 ID，请参阅"创建 [Azure Active Directory 应用"。](../get-started/add-aad-app-registration.md)</span><span class="sxs-lookup"><span data-stu-id="13ac0-136">**Note:** For details about how to register your app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>

## <a name="permission-scopes"></a><span data-ttu-id="13ac0-137">权限范围</span><span class="sxs-lookup"><span data-stu-id="13ac0-137">Permission Scopes</span></span>

<span data-ttu-id="13ac0-138">建议在初始化提供程序时将应用程序所需的所有权限范围添加到属性 (这 `scopes` 不适用于 [SharePoint 提供程序](../providers/sharepoint.md)) 。</span><span class="sxs-lookup"><span data-stu-id="13ac0-138">We recommend adding all the permission scopes your application needs to the `scopes` attribute or property when initializing your provider (this does not apply to the [SharePoint provider](../providers/sharepoint.md)).</span></span> <span data-ttu-id="13ac0-139">这是可选的，但会向用户显示单个许可屏幕，并包含应用内所有组件请求的权限聚合列表，而不是针对每个组件显示单独的屏幕，这可改善用户体验。</span><span class="sxs-lookup"><span data-stu-id="13ac0-139">This is optional, but will improve your user experience by presenting a single consent screen to the user with an aggregated list of permissions requested by all components in your app, rather than presenting separate screens for each component.</span></span> <span data-ttu-id="13ac0-140">以下示例显示如何使用 MsalProvider 进行此操作。</span><span class="sxs-lookup"><span data-stu-id="13ac0-140">The following examples show how to do this with the MsalProvider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

<span data-ttu-id="13ac0-141">如果要在代码中初始化提供程序，则提供属性中数组中的权限 `scopes` 范围。</span><span class="sxs-lookup"><span data-stu-id="13ac0-141">If you're initializing the provider in code, provide the permission scopes in an array in the `scopes` property.</span></span>

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

<span data-ttu-id="13ac0-142">您可以在每个组件的文档页的 **Microsoft Graph** 权限部分找到每个组件所需的权限范围列表。</span><span class="sxs-lookup"><span data-stu-id="13ac0-142">You can find the list of permission scopes required by each component in the **Microsoft Graph permissions** section of each component's documentation page.</span></span>

## <a name="provider-state"></a><span data-ttu-id="13ac0-143">提供程序状态</span><span class="sxs-lookup"><span data-stu-id="13ac0-143">Provider state</span></span>

<span data-ttu-id="13ac0-144">提供程序跟踪用户的身份验证状态，并通知组件。</span><span class="sxs-lookup"><span data-stu-id="13ac0-144">The provider keeps track of the user's authentication state and communicates it to the components.</span></span> <span data-ttu-id="13ac0-145">例如，当用户成功登录时，将更新为 ，向组件发出信号，指示他们现在可以调用 `ProviderState` `SignedIn` Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="13ac0-145">For example, when a user successfully signs in, the `ProviderState` is updated to `SignedIn`, signaling to the components that they are now able to make calls to Microsoft Graph.</span></span> <span data-ttu-id="13ac0-146">枚举 `ProviderState` 定义三种状态，如下所示。</span><span class="sxs-lookup"><span data-stu-id="13ac0-146">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

<span data-ttu-id="13ac0-147">在某些情况下，你将希望显示某些功能或仅在用户成功登录后执行某个操作。</span><span class="sxs-lookup"><span data-stu-id="13ac0-147">In some scenarios, you will want to show certain functionality or perform an action only after a user has successfully signed in.</span></span> <span data-ttu-id="13ac0-148">可以访问和检查提供程序状态，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="13ac0-148">You can access and check the provider state, as shown in the following example.</span></span>

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
<span data-ttu-id="13ac0-149">您也可以使用 `Providers.onProviderUpdated` 该方法在提供程序的状态发生更改时收到通知。</span><span class="sxs-lookup"><span data-stu-id="13ac0-149">You can also use the `Providers.onProviderUpdated` method to get notified whenever the state of the provider changes.</span></span>

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

## <a name="getting-an-access-token"></a><span data-ttu-id="13ac0-150">获取访问令牌</span><span class="sxs-lookup"><span data-stu-id="13ac0-150">Getting an access token</span></span>

<span data-ttu-id="13ac0-151">每个提供程序都公开一个调用的函数，该函数可以检索当前访问令牌或检索提供的范围 `getAccessToken` 的新访问令牌。</span><span class="sxs-lookup"><span data-stu-id="13ac0-151">Each provider exposes a function called `getAccessToken` that can retrieve the current access token or retrieve a new access token for the provided scopes.</span></span> <span data-ttu-id="13ac0-152">以下示例演示如何获取具有权限范围的新 `User.Read` 访问令牌。</span><span class="sxs-lookup"><span data-stu-id="13ac0-152">The following example shows how to get a new access token with the `User.Read` permission scope.</span></span>

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = Providers.globalProvider.getAccessToken({scopes: ['User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="13ac0-153">自行调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="13ac0-153">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="13ac0-154">所有组件都可以访问 Microsoft Graph，无需任何自定义，只要初始化提供程序 (如前面部分中所述) 。</span><span class="sxs-lookup"><span data-stu-id="13ac0-154">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous sections).</span></span> <span data-ttu-id="13ac0-155">如果要自行调用 Microsoft Graph，可以通过获取对组件使用的相同 Microsoft Graph SDK 的引用来实现此目标。</span><span class="sxs-lookup"><span data-stu-id="13ac0-155">If you want to make your own calls to Microsoft Graph, you can do so by getting a reference to the same Microsoft Graph SDK used by the components.</span></span> <span data-ttu-id="13ac0-156">首先，获取对全局的引用， `IProvider` 然后 `graph` 使用对象，如下所示：</span><span class="sxs-lookup"><span data-stu-id="13ac0-156">First, get a reference to the global `IProvider` and then use the `graph` object as shown:</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
<span data-ttu-id="13ac0-157">在某些情况下，可能需要传递其他权限，具体取决于你调用的 API。</span><span class="sxs-lookup"><span data-stu-id="13ac0-157">There might be cases where you need to pass additional permissions, depending on the API you're calling.</span></span> <span data-ttu-id="13ac0-158">以下示例说明了具体的操作方法。</span><span class="sxs-lookup"><span data-stu-id="13ac0-158">The following example shows how to do this.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a><span data-ttu-id="13ac0-159">使用多个提供程序</span><span class="sxs-lookup"><span data-stu-id="13ac0-159">Using multiple providers</span></span>

<span data-ttu-id="13ac0-160">在某些情况下，应用程序将在不同的环境中运行，并且每个环境都需要不同的提供程序。</span><span class="sxs-lookup"><span data-stu-id="13ac0-160">In some scenarios, your application will run in different environments and require a different provider for each.</span></span> <span data-ttu-id="13ac0-161">例如，应用可能同时作为 Web 应用程序和 Microsoft Teams 选项卡运行，这意味着你可能需要同时使用 MsalProvider 和 TeamsProvider。</span><span class="sxs-lookup"><span data-stu-id="13ac0-161">For example, the app might run as both a web application and a Microsoft Teams tab, which means you might need to use both the MsalProvider and the TeamsProvider.</span></span> <span data-ttu-id="13ac0-162">对于此方案，所有提供程序组件都有用于创建回退链的属性， `depends-on` 如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="13ac0-162">For this scenario, all provider components have the `depends-on` attribute to create a fallback chain, as shown in the following example.</span></span>

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

<span data-ttu-id="13ac0-163">在此方案中，仅在应用作为 Web 应用程序运行并且 TeamsProvider 在当前环境中不可用时，才使用 MsalProvider。</span><span class="sxs-lookup"><span data-stu-id="13ac0-163">In this scenario, the MsalProvider will only be used if your app is running as a web application and the TeamsProvider is not available in the current environment.</span></span>

<span data-ttu-id="13ac0-164">若要在代码中完成相同的任务，可以使用提供程序上的属性 `isAvailable` ，如下所示。</span><span class="sxs-lookup"><span data-stu-id="13ac0-164">To accomplish the same in code, you can use the `isAvailable` property on the provider, as shown.</span></span>

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```
## <a name="user-loginlogout"></a><span data-ttu-id="13ac0-165">用户登录/注销</span><span class="sxs-lookup"><span data-stu-id="13ac0-165">User Login/Logout</span></span>

<span data-ttu-id="13ac0-166">为应用程序初始化正确的提供程序后，可以添加 Toolkit 的 [登录](../components/login.md) 组件，以轻松快速地实现用户登录和注销。</span><span class="sxs-lookup"><span data-stu-id="13ac0-166">When you have the right providers initialized for your application, you can add the Toolkit's [Login component](../components/login.md) to easily and quickly implement user login and logout.</span></span> <span data-ttu-id="13ac0-167">该组件与提供程序一起处理所有身份验证逻辑和登录/注销功能。</span><span class="sxs-lookup"><span data-stu-id="13ac0-167">The component works with the provider to handle all of the authentication logic and login/logout functionality.</span></span> <span data-ttu-id="13ac0-168">以下示例使用 MsalProvider 和 Login 组件。</span><span class="sxs-lookup"><span data-stu-id="13ac0-168">The following example uses the MsalProvider and the Login component.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="13ac0-169">在你想要自己实现此方案的情况下，而不是使用 Toolkit 的 Login 组件，可以通过使用提供程序的方法和方法来 `login` `logout` 实现。</span><span class="sxs-lookup"><span data-stu-id="13ac0-169">In scenarios where you want to implement this yourself, rather than using the Toolkit's Login component, you can do so by using the `login` and `logout` methods of the provider.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="13ac0-170">实现你自己的提供程序</span><span class="sxs-lookup"><span data-stu-id="13ac0-170">Implement your own provider</span></span>

<span data-ttu-id="13ac0-171">在您希望将 Toolkit组件添加到具有预先存在的身份验证代码的应用程序的方案中，您可以创建一个连接到身份验证机制的自定义提供程序，而不是使用预定义的提供程序。</span><span class="sxs-lookup"><span data-stu-id="13ac0-171">In scenarios where you want to add Toolkit components to an application with pre-existing authentication code, you can create a custom provider that hooks into your authentication mechanism, instead of using our predefined providers.</span></span> <span data-ttu-id="13ac0-172">该工具包提供了两种创建新提供程序的方法：</span><span class="sxs-lookup"><span data-stu-id="13ac0-172">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="13ac0-173">创建一 `SimpleProvider` 个通过传递函数从身份验证代码返回访问令牌的新令牌。</span><span class="sxs-lookup"><span data-stu-id="13ac0-173">Create a new `SimpleProvider` that returns an access token from your authentication code by passing in a function.</span></span>
- <span data-ttu-id="13ac0-174">扩展 `IProvider` 抽象类。</span><span class="sxs-lookup"><span data-stu-id="13ac0-174">Extend the `IProvider` abstract class.</span></span>

<span data-ttu-id="13ac0-175">有关每个提供程序的更多详细信息，请参阅 [自定义提供程序](../providers/custom.md)。</span><span class="sxs-lookup"><span data-stu-id="13ac0-175">For more details about each one, see [custom providers](../providers/custom.md).</span></span>
