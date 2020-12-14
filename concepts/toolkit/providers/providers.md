---
title: Microsoft Graph Toolkit提供程序
description: Microsoft Graph Toolkit提供程序支持所有组件的身份验证和 Microsoft Graph 访问。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: a4cd1b58bb29e42ecb0283709e71a3ce3a7e86d7
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658233"
---
# <a name="microsoft-graph-toolkit-providers"></a>Microsoft Graph Toolkit提供程序

Microsoft Graph Toolkit提供程序使应用程序能够使用 Microsoft Identity 进行身份验证，并且只需几行代码就访问 Microsoft Graph。 每个提供程序都处理用户身份验证和获取访问令牌以调用 Microsoft Graph API，因此你不必自己编写此代码。 

你可以自行使用提供程序（无需组件）为应用快速实现身份验证，并可通过 JavaScript 客户端 SDK 调用 Microsoft Graph。

当使用 Microsoft Graph Toolkit组件访问 Microsoft Graph 时，提供程序是必需的。 如果已有自己的身份验证并且想要使用组件，可以改为使用 [自定义](./custom.md) 提供程序。

该Toolkit包括以下提供程序。

|提供程序|说明|
|---------|-----------|
|[Msal](./msal.md)|使用 MSAL.js 登录用户并获取令牌以在 Web 应用程序中与 Microsoft Graph 一同使用。|
|[SharePoint](./sharepoint.md)|对 SharePoint Web 部件内的组件进行身份验证并提供 Microsoft Graph 访问。|
|[Teams](./teams.md)|对 Microsoft Teams 选项卡中的组件进行身份验证并提供 Microsoft Graph 访问权限。|
|[代理](./proxy.md)|允许通过后端路由对 Microsoft Graph 的所有调用来使用后端身份验证。|
|[自定义](./custom.md)|创建自定义提供程序以使用应用程序的现有身份验证代码启用身份验证并访问 Microsoft Graph。|

## <a name="initializing-a-provider"></a>初始化提供程序

若要在应用中使用提供程序，需要初始化新提供程序，然后在提供程序命名空间中将提供程序设置为全局提供程序。 我们建议在开始使用任何组件之前执行此操作。 可以通过两种方法之一执行此操作：

**选项 1：使用提供程序组件**

可以直接在 HTML 中使用该提供程序的组件版本。 在后台，将初始化新提供程序并设置为全局提供程序。 以下示例演示如何使用 MsalProvider。

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

**选项 2：在代码中初始化**

通过 JavaScript 代码初始化提供程序，可以提供更多选项。 为此，请创建一个新的提供程序实例，并设置要使用的提供程序的 `Providers.globalProvider` 属性值。 以下示例演示如何使用 MsalProvider。

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> **注意：** 若要详细了解如何注册应用和获取客户端 ID，请参阅"创建 [Azure Active Directory 应用"。](../get-started/add-aad-app-registration.md)

## <a name="permission-scopes"></a>权限范围

建议在初始化提供程序时，将应用程序需要的所有权限范围添加到属性 (这不适用于 `scopes` [SharePoint 提供程序](../providers/sharepoint.md)) 。 这是可选的，但会通过向用户显示单个许可屏幕，并包含应用内所有组件请求的权限的聚合列表，而不是针对每个组件显示单独的屏幕，来改进用户体验。 以下示例显示如何使用 MsalProvider 进行此操作。

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

如果要在代码中初始化提供程序，请提供属性中数组中的权限 `scopes` 范围。

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

您可以在每个组件的文档页的 **Microsoft Graph** 权限部分找到每个组件所需的权限范围列表。

## <a name="provider-state"></a>提供程序状态

提供程序跟踪用户的身份验证状态，并告知组件。 例如，当用户成功登录时，会更新为 ，向组件发出信号，指示他们现在可以调用 `ProviderState` `SignedIn` Microsoft Graph。 枚举 `ProviderState` 定义三种状态，如下所示。

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

在某些情况下，仅在用户成功登录后，才希望显示某些功能或执行此操作。 可以访问和检查提供程序状态，如以下示例所示。

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
您还可以使用 `Providers.onProviderUpdated` 该方法在提供程序的状态发生更改时收到通知。

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

## <a name="getting-an-access-token"></a>获取访问令牌

每个提供程序都公开一个调用的函数，该函数可以检索当前访问令牌或检索提供的范围 `getAccessToken` 的新访问令牌。 以下示例演示如何获取具有权限范围的新 `User.Read` 访问令牌。

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = Provider.globalProvider.getAccessToken({scopes: 'User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a>自行调用 Microsoft Graph

所有组件都可以访问 Microsoft Graph，无需任何自定义，只要初始化提供程序 (如前面的部分所述) 。 如果要自行调用 Microsoft Graph，可以通过获取对组件使用的同一 Microsoft Graph SDK 的引用来实现此目标。 首先，获取对全局的引用 `IProvider` ，然后 `graph` 使用对象，如下所示：

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
在某些情况下，可能需要传递其他权限，具体取决于你调用的 API。 以下示例说明了具体的操作方法。

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a>使用多个提供程序

在某些情况下，应用程序将在不同的环境中运行，并且每个环境都需要不同的提供程序。 例如，应用可能同时作为 Web 应用程序和 Microsoft Teams 选项卡运行，这意味着你可能需要同时使用 MsalProvider 和 TeamsProvider。 对于此方案，所有提供程序组件都有用于创建回退链的属性， `depends-on` 如以下示例所示。

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

在此方案中，仅在应用作为 Web 应用程序运行且 TeamsProvider 在当前环境中不可用时，才使用 MsalProvider。

若要在代码中完成相同的任务，可以使用提供程序上的 `isAvailable` 属性，如下所示。

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```
## <a name="user-loginlogout"></a>用户登录/注销

为应用程序初始化正确的提供程序后，可以添加 Toolkit 的 [登录](../components/login.md) 组件，以轻松快速地实现用户登录和注销。 该组件与提供程序一起处理所有身份验证逻辑和登录/注销功能。 以下示例使用 MsalProvider 和 Login 组件。

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
<mgt-login></mgt-login>
```

在你想要自己实现此操作（而不是使用 Toolkit 的 Login 组件）的情况下，可以使用提供程序的方法和方法来 `login` `logout` 实现此操作。

## <a name="implement-your-own-provider"></a>实现你自己的提供程序

在想要将 Toolkit 组件添加到具有预先存在的身份验证代码的应用程序的方案中，您可以创建一个连接到身份验证机制的自定义提供程序，而不是使用预定义的提供程序。 该工具包提供两种创建新提供程序的方法：

- 创建一 `SimpleProvider` 个通过传递函数从身份验证代码返回访问令牌的新令牌。
- 扩展 `IProvider` 抽象类。

有关每个提供程序的更多详细信息，请参阅 [自定义提供程序](../providers/custom.md)。
