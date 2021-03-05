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
# <a name="microsoft-graph-toolkit-providers"></a>Microsoft Graph Toolkit提供程序

Microsoft Graph Toolkit提供程序使应用程序能够使用 Microsoft Identity 进行身份验证，并且只需几行代码访问 Microsoft Graph。 每个提供程序都处理用户身份验证并获取访问令牌以调用 Microsoft Graph API，这样你不必自己编写此代码。 

你可以自行使用提供程序，而无需使用组件，以快速实现应用的身份验证，并可以通过 JavaScript 客户端 SDK 调用 Microsoft Graph。

使用 Microsoft Graph Toolkit组件时，提供程序是必需的，因为组件使用它们来访问 Microsoft Graph。 如果你已拥有自己的身份验证并且想要使用组件，可以改为使用 [自定义](./custom.md) 提供程序。

该Toolkit包括以下提供程序。

|提供程序|说明|
|---------|-----------|
|[Msal](./msal.md)|使用MSAL.js登录用户并获取令牌以在 Web 应用程序中与 Microsoft Graph 一同使用。|
|[都云](./electron.md)|验证并提供对"一线"应用内组件的 Microsoft Graph 访问。|
|[SharePoint](./sharepoint.md)|对 SharePoint Web 部件内的组件进行身份验证并提供 Microsoft Graph 访问。|
|[Teams](./teams.md)|对 Microsoft Teams 选项卡内的组件进行身份验证并提供 Microsoft Graph 访问权限。|
|[代理](./proxy.md)|允许通过后端路由对 Microsoft Graph 的所有调用来使用后端身份验证。|
|[自定义](./custom.md)|创建自定义提供程序以使用应用程序的现有身份验证代码启用身份验证并访问 Microsoft Graph。|

## <a name="initializing-a-provider"></a>初始化提供程序

若要在应用中使用提供程序，需要初始化新提供程序，然后在提供程序命名空间中将提供程序设置为全局提供程序。 建议在开始使用任何组件之前执行此操作。 可以通过两种方法之一执行此操作：

**选项 1：使用提供程序组件**

可以直接在 HTML 中使用该提供程序的组件版本。 在后台，将初始化新提供程序并设置为全局提供程序。 以下示例演示如何使用 MsalProvider。

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

**选项 2：在代码中初始化**

在 JavaScript 代码中初始化提供程序使您能够提供更多选项。 为此，请创建新的提供程序实例，将属性的值设置为要 `Providers.globalProvider` 使用的提供程序。 以下示例演示如何使用 MsalProvider。

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> **注意：** 若要详细了解如何注册应用和获取客户端 ID，请参阅"创建 [Azure Active Directory 应用"。](../get-started/add-aad-app-registration.md)

## <a name="permission-scopes"></a>权限范围

建议在初始化提供程序时将应用程序所需的所有权限范围添加到属性 (这 `scopes` 不适用于 [SharePoint 提供程序](../providers/sharepoint.md)) 。 这是可选的，但会向用户显示单个许可屏幕，并包含应用内所有组件请求的权限聚合列表，而不是针对每个组件显示单独的屏幕，这可改善用户体验。 以下示例显示如何使用 MsalProvider 进行此操作。

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

如果要在代码中初始化提供程序，则提供属性中数组中的权限 `scopes` 范围。

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

您可以在每个组件的文档页的 **Microsoft Graph** 权限部分找到每个组件所需的权限范围列表。

## <a name="provider-state"></a>提供程序状态

提供程序跟踪用户的身份验证状态，并通知组件。 例如，当用户成功登录时，将更新为 ，向组件发出信号，指示他们现在可以调用 `ProviderState` `SignedIn` Microsoft Graph。 枚举 `ProviderState` 定义三种状态，如下所示。

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

在某些情况下，你将希望显示某些功能或仅在用户成功登录后执行某个操作。 可以访问和检查提供程序状态，如以下示例所示。

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
您也可以使用 `Providers.onProviderUpdated` 该方法在提供程序的状态发生更改时收到通知。

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
  const token = Providers.globalProvider.getAccessToken({scopes: ['User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a>自行调用 Microsoft Graph

所有组件都可以访问 Microsoft Graph，无需任何自定义，只要初始化提供程序 (如前面部分中所述) 。 如果要自行调用 Microsoft Graph，可以通过获取对组件使用的相同 Microsoft Graph SDK 的引用来实现此目标。 首先，获取对全局的引用， `IProvider` 然后 `graph` 使用对象，如下所示：

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

在此方案中，仅在应用作为 Web 应用程序运行并且 TeamsProvider 在当前环境中不可用时，才使用 MsalProvider。

若要在代码中完成相同的任务，可以使用提供程序上的属性 `isAvailable` ，如下所示。

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

在你想要自己实现此方案的情况下，而不是使用 Toolkit 的 Login 组件，可以通过使用提供程序的方法和方法来 `login` `logout` 实现。

## <a name="implement-your-own-provider"></a>实现你自己的提供程序

在您希望将 Toolkit组件添加到具有预先存在的身份验证代码的应用程序的方案中，您可以创建一个连接到身份验证机制的自定义提供程序，而不是使用预定义的提供程序。 该工具包提供了两种创建新提供程序的方法：

- 创建一 `SimpleProvider` 个通过传递函数从身份验证代码返回访问令牌的新令牌。
- 扩展 `IProvider` 抽象类。

有关每个提供程序的更多详细信息，请参阅 [自定义提供程序](../providers/custom.md)。
