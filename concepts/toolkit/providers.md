---
title: Microsoft Graph 工具包提供程序
description: Microsoft Graph 工具包提供程序为所有组件启用身份验证和 Microsoft Graph 访问。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 4b51fdf91fd37c0c3dc5ea0ec49571a8ed4e5d47
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086645"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="6b159-103">Microsoft Graph 工具包提供程序</span><span class="sxs-lookup"><span data-stu-id="6b159-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="6b159-104">Microsoft Graph 工具包提供程序使应用程序能够使用 Microsoft Identity 进行身份验证，并在仅几行代码中访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="6b159-104">The Microsoft Graph Toolkit providers enable your application to authenticate with Microsoft Identity and access Microsoft Graph in only few lines of code.</span></span> <span data-ttu-id="6b159-105">每个提供程序处理用户身份验证并获取访问令牌以调用 Microsoft Graph Api，因此您无需自己编写此代码。</span><span class="sxs-lookup"><span data-stu-id="6b159-105">Each provider handles user authentication and acquiring the access tokens to call Microsoft Graph APIs, so that you don't have to write this code yourself.</span></span> 

<span data-ttu-id="6b159-106">您可以使用自己的提供程序（不含组件）快速为您的应用程序实现身份验证，并通过 JavaScript 客户端 SDK 调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="6b159-106">You can use the providers on their own, without components, to quickly implement authentication for your app and make calls to Microsoft Graph via the JavaScript client SDK.</span></span>

<span data-ttu-id="6b159-107">使用 Microsoft Graph 工具包组件时，这些提供程序是必需的，因为组件使用它们来访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="6b159-107">The providers are required when using the Microsoft Graph Toolkit components as the components use them to access Microsoft Graph.</span></span> <span data-ttu-id="6b159-108">如果您已经有自己的身份验证并且想要使用组件，则可以改为使用 [自定义提供程序](./providers/custom.md) 。</span><span class="sxs-lookup"><span data-stu-id="6b159-108">If you already have your own authentication and want to use the components, you can use a [custom provider](./providers/custom.md) instead.</span></span>

<span data-ttu-id="6b159-109">该工具包包括以下提供程序。</span><span class="sxs-lookup"><span data-stu-id="6b159-109">The Toolkit includes the following providers.</span></span>

|<span data-ttu-id="6b159-110">提供程序</span><span class="sxs-lookup"><span data-stu-id="6b159-110">Providers</span></span>|<span data-ttu-id="6b159-111">说明</span><span class="sxs-lookup"><span data-stu-id="6b159-111">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="6b159-112">Msal</span><span class="sxs-lookup"><span data-stu-id="6b159-112">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="6b159-113">使用 MSAL.js 在 web 应用程序中登录用户和获取令牌以与 Microsoft Graph 一起使用。</span><span class="sxs-lookup"><span data-stu-id="6b159-113">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph in a web application.</span></span>|
|[<span data-ttu-id="6b159-114">SharePoint</span><span class="sxs-lookup"><span data-stu-id="6b159-114">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="6b159-115">对 SharePoint web 部件内的组件进行身份验证并提供 Microsoft Graph 访问权限。</span><span class="sxs-lookup"><span data-stu-id="6b159-115">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="6b159-116">Teams</span><span class="sxs-lookup"><span data-stu-id="6b159-116">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="6b159-117">对 Microsoft 团队选项卡中的组件进行身份验证和提供 Microsoft Graph 访问。</span><span class="sxs-lookup"><span data-stu-id="6b159-117">Authenticates and provides Microsoft Graph access to components inside  Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="6b159-118">代理</span><span class="sxs-lookup"><span data-stu-id="6b159-118">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="6b159-119">通过将对 Microsoft Graph 的所有调用通过后端路由，允许使用后端身份验证。</span><span class="sxs-lookup"><span data-stu-id="6b159-119">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="6b159-120">自定义</span><span class="sxs-lookup"><span data-stu-id="6b159-120">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="6b159-121">创建自定义提供程序，以便通过应用程序的现有身份验证代码启用对 Microsoft Graph 的身份验证和访问。</span><span class="sxs-lookup"><span data-stu-id="6b159-121">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="initializing-a-provider"></a><span data-ttu-id="6b159-122">初始化提供程序</span><span class="sxs-lookup"><span data-stu-id="6b159-122">Initializing a provider</span></span>

<span data-ttu-id="6b159-123">若要在应用程序中使用提供程序，您需要初始化一个新的提供程序，然后将其设置为 provider 命名空间中的全局提供程序。</span><span class="sxs-lookup"><span data-stu-id="6b159-123">To use a provider in your app, you need to initialize a new provider and then set it as the global provider in the Providers namespace.</span></span> <span data-ttu-id="6b159-124">我们建议您在开始使用任何组件之前执行此操作。</span><span class="sxs-lookup"><span data-stu-id="6b159-124">We recommend doing this before you start using any of the components.</span></span> <span data-ttu-id="6b159-125">可以通过以下两种方式之一执行此操作：</span><span class="sxs-lookup"><span data-stu-id="6b159-125">You can do this one of two ways:</span></span>

<span data-ttu-id="6b159-126">**选项1：使用提供程序组件**</span><span class="sxs-lookup"><span data-stu-id="6b159-126">**Option 1: Use the provider component**</span></span>

<span data-ttu-id="6b159-127">您可以直接在 HTML 中使用提供程序的组件版本。</span><span class="sxs-lookup"><span data-stu-id="6b159-127">You can use the component version of the provider directly in your HTML.</span></span> <span data-ttu-id="6b159-128">在幕后，将初始化新的提供程序并将其设置为全局提供程序。</span><span class="sxs-lookup"><span data-stu-id="6b159-128">Behind the scenes, a new provider is initialized and set as the global provider.</span></span> <span data-ttu-id="6b159-129">下面的示例演示如何使用 MsalProvider。</span><span class="sxs-lookup"><span data-stu-id="6b159-129">The following example shows how to use the MsalProvider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

<span data-ttu-id="6b159-130">**选项2：在代码中初始化**</span><span class="sxs-lookup"><span data-stu-id="6b159-130">**Option 2: Initialize in code**</span></span>

<span data-ttu-id="6b159-131">通过在 JavaScript 代码中初始化提供程序，可以提供更多的选项。</span><span class="sxs-lookup"><span data-stu-id="6b159-131">Initializing your provider in your JavaScript code enables you to provide more options.</span></span> <span data-ttu-id="6b159-132">为此，请创建一个新的提供程序实例，并将该属性的值设置 `Providers.globalProvider` 为您想要使用的提供程序。</span><span class="sxs-lookup"><span data-stu-id="6b159-132">To do this, create a new provider instance and set the value of the `Providers.globalProvider` property to the provider you'd like to use.</span></span> <span data-ttu-id="6b159-133">下面的示例演示如何使用 MsalProvider。</span><span class="sxs-lookup"><span data-stu-id="6b159-133">The following example shows how to use the MsalProvider.</span></span>

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> <span data-ttu-id="6b159-134">**注意：** 有关如何注册您的应用程序并获取客户端 ID 的详细信息，请参阅 [Create a Azure Active Directory app](./get-started/add-aad-app-registration.md)。</span><span class="sxs-lookup"><span data-stu-id="6b159-134">**Note:** For details about how to register your app and get a client ID, see [Create an Azure Active Directory app](./get-started/add-aad-app-registration.md).</span></span>

## <a name="permission-scopes"></a><span data-ttu-id="6b159-135">权限范围</span><span class="sxs-lookup"><span data-stu-id="6b159-135">Permission Scopes</span></span>

<span data-ttu-id="6b159-136">建议在初始化提供程序时添加应用程序需要的所有权限范围， `scopes` (此属性不应用于 [SharePoint 提供程序](./providers/sharepoint.md)) 。</span><span class="sxs-lookup"><span data-stu-id="6b159-136">We recommend adding all the permission scopes your application needs to the `scopes` attribute or property when initializing your provider (this does not apply to the [SharePoint provider](./providers/sharepoint.md)).</span></span> <span data-ttu-id="6b159-137">这是可选的，但将通过向用户提供应用程序中所有组件请求的权限的聚合列表，而不是为每个组件呈现单独的屏幕，来改善用户体验。</span><span class="sxs-lookup"><span data-stu-id="6b159-137">This is optional, but will improve your user experience by presenting a single consent screen to the user with an aggregated list of permissions requested by all components in your app, rather than presenting separate screens for each component.</span></span> <span data-ttu-id="6b159-138">下面的示例演示如何使用 MsalProvider 执行此操作。</span><span class="sxs-lookup"><span data-stu-id="6b159-138">The following examples show how to do this with the MsalProvider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

<span data-ttu-id="6b159-139">如果要在代码中初始化提供程序，请在属性中提供数组中的权限范围 `scopes` 。</span><span class="sxs-lookup"><span data-stu-id="6b159-139">If you're initializing the provider in code, provide the permission scopes in an array in the `scopes` property.</span></span>

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

<span data-ttu-id="6b159-140">可以在每个组件的 "文档" 页的 " **Microsoft Graph 权限** " 一节中找到每个组件所需的权限范围列表。</span><span class="sxs-lookup"><span data-stu-id="6b159-140">You can find the list of permission scopes required by each component in the **Microsoft Graph permissions** section of each component's documentation page.</span></span>

## <a name="provider-state"></a><span data-ttu-id="6b159-141">提供程序状态</span><span class="sxs-lookup"><span data-stu-id="6b159-141">Provider state</span></span>

<span data-ttu-id="6b159-142">提供程序跟踪用户的身份验证状态并将其传递到组件。</span><span class="sxs-lookup"><span data-stu-id="6b159-142">The provider keeps track of the user's authentication state and communicates it to the components.</span></span> <span data-ttu-id="6b159-143">例如，当用户成功登录时，将 `ProviderState` 更新为 `SignedIn` ，向这些组件发出信号，通知他们现在可以调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="6b159-143">For example, when a user successfully signs in, the `ProviderState` is updated to `SignedIn`, signaling to the components that they are now able to make calls to Microsoft Graph.</span></span> <span data-ttu-id="6b159-144">`ProviderState`枚举定义三种状态，如下所示。</span><span class="sxs-lookup"><span data-stu-id="6b159-144">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

<span data-ttu-id="6b159-145">在某些情况下，您可能需要显示特定功能或仅在用户成功登录后执行某项操作。</span><span class="sxs-lookup"><span data-stu-id="6b159-145">In some scenarios, you will want to show certain functionality or perform an action only after a user has successfully signed in.</span></span> <span data-ttu-id="6b159-146">您可以访问和检查提供程序状态，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="6b159-146">You can access and check the provider state, as shown in the following example.</span></span>

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
<span data-ttu-id="6b159-147">您还可以使用 `Providers.onProviderUpdated` 方法在提供程序的状态更改时收到通知。</span><span class="sxs-lookup"><span data-stu-id="6b159-147">You can also use the `Providers.onProviderUpdated` method to get notified whenever the state of the provider changes.</span></span>

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

## <a name="getting-an-access-token"></a><span data-ttu-id="6b159-148">获取访问令牌</span><span class="sxs-lookup"><span data-stu-id="6b159-148">Getting an access token</span></span>

<span data-ttu-id="6b159-149">每个提供程序公开一个调用 `getAccessToken` 的函数，该函数可以检索当前访问令牌或检索提供的作用域的新访问令牌。</span><span class="sxs-lookup"><span data-stu-id="6b159-149">Each provider exposes a function called `getAccessToken` that can retreive the current access token or retrieve a new access token for the provided scopes.</span></span> <span data-ttu-id="6b159-150">下面的示例演示如何获取具有权限范围的新访问令牌 `User.Read` 。</span><span class="sxs-lookup"><span data-stu-id="6b159-150">The following example shows how to get a new access token with the `User.Read` permission scope.</span></span>

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = Provider.globalProvider.getAccessToken({scopes: 'User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="6b159-151">对 Microsoft Graph 进行自己的调用</span><span class="sxs-lookup"><span data-stu-id="6b159-151">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="6b159-152">所有组件都可以访问 Microsoft Graph，而无需进行任何自定义，只要您初始化提供程序 (如上一节) 中所述。</span><span class="sxs-lookup"><span data-stu-id="6b159-152">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous sections).</span></span> <span data-ttu-id="6b159-153">如果要对 Microsoft Graph 进行自己的调用，可以通过获取对组件使用的相同 Microsoft Graph SDK 的引用来执行此操作。</span><span class="sxs-lookup"><span data-stu-id="6b159-153">If you want to make your own calls to Microsoft Graph, you can do so by getting a reference to the same Microsoft Graph SDK used by the components.</span></span> <span data-ttu-id="6b159-154">首先，获取对全局的引用 `IProvider` ，然后按 `graph` 如下所示使用对象：</span><span class="sxs-lookup"><span data-stu-id="6b159-154">First, get a reference to the global `IProvider` and then use the `graph` object as shown:</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
<span data-ttu-id="6b159-155">在某些情况下，您可能需要传递其他权限，具体取决于您要调用的 API。</span><span class="sxs-lookup"><span data-stu-id="6b159-155">There might be cases where you need to pass additional permissions, depending on the API you're calling.</span></span> <span data-ttu-id="6b159-156">以下示例说明了具体的操作方法。</span><span class="sxs-lookup"><span data-stu-id="6b159-156">The following example shows how to do this.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a><span data-ttu-id="6b159-157">使用多个提供程序</span><span class="sxs-lookup"><span data-stu-id="6b159-157">Using multiple providers</span></span>

<span data-ttu-id="6b159-158">在某些情况下，您的应用程序将在不同的环境中运行，每个都需要不同的提供程序。</span><span class="sxs-lookup"><span data-stu-id="6b159-158">In some scenarios, your application will run in different environments and require a different provider for each.</span></span> <span data-ttu-id="6b159-159">例如，应用程序可能同时作为 web 应用程序和 Microsoft 团队选项卡运行，这意味着您可能需要同时使用 MsalProvider 和 TeamsProvider。</span><span class="sxs-lookup"><span data-stu-id="6b159-159">For example, the app might run as both a web application and a Microsoft Teams tab, which means you might need to use both the MsalProvider and the TeamsProvider.</span></span> <span data-ttu-id="6b159-160">对于此方案，所有提供程序组件都具有 `depends-on` 创建回退链的属性，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="6b159-160">For this scenario, all provider components have the `depends-on` attribute to create a fallback chain, as shown in the following example.</span></span>

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

<span data-ttu-id="6b159-161">在这种情况下，仅当应用程序作为 web 应用程序运行，并且 TeamsProvider 在当前环境中不可用时，才会使用 MsalProvider。</span><span class="sxs-lookup"><span data-stu-id="6b159-161">In this scenario, the MsalProvider will only be used if your app is running as a web application and the TeamsProvider is not available in the current environment.</span></span>

<span data-ttu-id="6b159-162">若要在代码中实现相同，可以使用 `isAvailable` 提供程序上的属性，如下所示。</span><span class="sxs-lookup"><span data-stu-id="6b159-162">To accomplish the same in code, you can use the `isAvailable` property on the provider, as shown.</span></span>

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```
## <a name="user-loginlogout"></a><span data-ttu-id="6b159-163">用户登录/注销</span><span class="sxs-lookup"><span data-stu-id="6b159-163">User Login/Logout</span></span>

<span data-ttu-id="6b159-164">如果为应用程序初始化了正确的提供程序，则可以添加该工具包的 [登录组件](./components/login.md) ，以便轻松快速地实现用户登录和注销。</span><span class="sxs-lookup"><span data-stu-id="6b159-164">When you have the right providers initialized for your application, you can add the Toolkit's [Login component](./components/login.md) to easily and quickly implement user login and logout.</span></span> <span data-ttu-id="6b159-165">组件与提供程序配合使用，以处理所有身份验证逻辑和登录/注销功能。</span><span class="sxs-lookup"><span data-stu-id="6b159-165">The component works with the provider to handle all of the authentication logic and login/logout functionality.</span></span> <span data-ttu-id="6b159-166">下面的示例使用 MsalProvider 和 Login 组件。</span><span class="sxs-lookup"><span data-stu-id="6b159-166">The following example uses the MsalProvider and the Login component.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="6b159-167">在您希望自己实现这一点的方案中，您可以使用 `login` 提供程序的和方法来执行此操作，而不是使用该工具包的登录组件 `logout` 。</span><span class="sxs-lookup"><span data-stu-id="6b159-167">In scenarios where you want to implement this yourself, rather than using the Toolkit's Login component, you can do so by using the `login` and `logout` methods of the provider.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="6b159-168">实现您自己的提供程序</span><span class="sxs-lookup"><span data-stu-id="6b159-168">Implement your own provider</span></span>

<span data-ttu-id="6b159-169">在要将工具包组件添加到具有预先存在的身份验证代码的应用程序的方案中，您可以创建一个挂接到您的身份验证机制中的自定义提供程序，而不是使用预定义的提供程序。</span><span class="sxs-lookup"><span data-stu-id="6b159-169">In scenarios where you want to add Toolkit components to an application with pre-existing authentication code, you can create a custom provider that hooks into your authentication mechanism, instead of using our predefined providers.</span></span> <span data-ttu-id="6b159-170">该工具包提供了两种创建新的提供程序的方法：</span><span class="sxs-lookup"><span data-stu-id="6b159-170">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="6b159-171">创建一个新 `SimpleProvider` 的，它通过传入函数返回身份验证代码中的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="6b159-171">Create a new `SimpleProvider` that returns an access token from your authentication code by passing in a function.</span></span>
- <span data-ttu-id="6b159-172">扩展 `IProvider` 抽象类。</span><span class="sxs-lookup"><span data-stu-id="6b159-172">Extend the `IProvider` abstract class.</span></span>

<span data-ttu-id="6b159-173">有关每个的详细信息，请参阅 [自定义提供程序](./providers/custom.md)。</span><span class="sxs-lookup"><span data-stu-id="6b159-173">For more details about each one, see [custom providers](./providers/custom.md).</span></span>
