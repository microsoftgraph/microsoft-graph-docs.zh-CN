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
# <a name="microsoft-graph-toolkit-providers"></a>Microsoft Graph Toolkit提供程序

Microsoft Graph Toolkit提供程序使应用程序能够使用 Microsoft 标识进行身份验证，并且只需几Graph几行代码Graph访问 Microsoft 标识。 每个提供程序都处理用户身份验证并获取访问令牌以调用 Microsoft Graph API，因此，你不必自己编写此代码。 

你可以自行使用提供程序（无需组件）为应用快速实现身份验证，并调用 Microsoft Graph JavaScript 客户端 SDK。

使用 Microsoft Graph Toolkit组件时，提供程序是必需的，因为组件使用它们访问 Microsoft Graph。 如果你已拥有自己的身份验证并且想要使用组件，可以改为使用 [自定义提供程序](./custom.md) 。

该Toolkit包括以下提供程序。

|提供程序|说明|
|---------|-----------|
|[Msal](./msal.md)|使用 MSAL.js 登录用户并获取与 Web 应用程序中的 Microsoft Graph一同使用的令牌。|
|[Msal 2.0](./msal2.md)| 使用 msal-browser 登录用户并获取令牌，以便与 Web Graph Microsoft 应用程序一同使用。 | 
|[百年](./electron.md)|通过身份验证并提供 Microsoft Graph访问在一些应用内的组件。|
|[SharePoint](./sharepoint.md)|通过身份验证并提供 Microsoft Graph访问 Web 部件内SharePoint权限。|
|[Teams](./teams.md)|通过身份验证并提供 Microsoft Graph访问选项卡内Microsoft Teams权限。|
|[代理](./proxy.md)|允许通过后端将所有调用路由到 Microsoft Graph后端身份验证。|
|[自定义](./custom.md)|创建自定义提供程序以使用应用程序的现有身份验证代码Graph访问 Microsoft 客户端。|

## <a name="initializing-a-provider"></a>初始化提供程序

若要在应用中使用提供程序，你需要初始化一个新提供程序，然后在 Providers 命名空间中将它设置为全局提供程序。 我们建议在开始使用任何组件之前执行此操作。 可以通过两种方法之一执行此工作：

**选项 1：使用提供程序组件**

可以直接在 HTML 中使用该提供程序的组件版本。 在后台，将初始化新的提供程序并设置为全局提供程序。 以下示例演示如何使用 Msal2Provider。

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="YOUR_CLIENT_ID"></mgt-msal2-provider>
```

**选项 2：在代码中初始化**

通过 JavaScript 代码初始化提供程序，可以提供更多选项。 为此，请创建一个新的提供程序实例，将属性的值设置为 `Providers.globalProvider` 希望使用的提供程序。 以下示例演示如何使用 Msal2Provider。

```js
import {Providers, Msal2Provider } from "@microsoft/mgt";
Providers.globalProvider = new Msal2Provider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> **注意：** 若要详细了解如何注册应用和获取客户端 ID，请参阅创建Azure Active Directory [应用](../get-started/add-aad-app-registration.md)。

## <a name="permission-scopes"></a>权限范围

建议在初始化提供程序时将应用程序需要的所有权限范围添加到属性或属性 (这不适用于 SharePoint `scopes` [提供程序](../providers/sharepoint.md)) 。 这是可选的，但会通过向用户显示单个许可屏幕（即应用内所有组件请求的权限聚合列表）来改进用户体验，而不是显示每个组件的单独屏幕。 以下示例显示如何使用 Msal2Provider 进行此操作。

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal2-provider>
```

如果要在代码中初始化提供程序，请提供 属性中数组中 `scopes` 的权限范围。

```js
import {Providers, Msal2Provider } from "@microsoft/mgt";
Providers.globalProvider = new Msal2Provider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

您可以在每个组件的文档页的 Microsoft Graph **权限** 部分找到每个组件所需的权限范围列表。

## <a name="provider-state"></a>提供程序状态

提供程序跟踪用户的身份验证状态，并通知组件。 例如，当用户成功登录时，将 更新为 ，向 组件发出信号，指示他们现在可以调用 `ProviderState` `SignedIn` Microsoft Graph。 枚举 `ProviderState` 定义三种状态，如下所示。

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
您还可以使用 `Providers.onProviderUpdated` 方法在提供程序的状态发生更改时收到通知。

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

每个提供程序都公开一个称为 的函数，该函数可以检索当前访问令牌或检索提供的范围 `getAccessToken` 的新访问令牌。 以下示例演示如何获取具有权限范围的新访问 `User.Read` 令牌。

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = await Providers.globalProvider.getAccessToken({scopes: ['User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a>自行调用 Microsoft Graph

所有组件都可以访问 Microsoft Graph，而无需任何自定义，只要初始化提供程序 (如前面的部分所述) 。 如果要自行调用 Microsoft Graph，可以通过获取对组件使用的同一 Microsoft Graph SDK 的引用来这样做。 首先，获取对全局的引用 `IProvider` ，然后 `graph` 使用 对象，如下所示：

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

在某些情况下，应用程序将在不同的环境中运行，并且需要针对每个环境使用不同的提供程序。 例如，应用可能同时作为 Web 应用程序和 Microsoft Teams 选项卡运行，这意味着你可能需要同时使用 Msal2Provider 和 TeamsProvider。 对于此方案，所有提供程序组件都有 用于创建回退链的属性， `depends-on` 如以下示例所示。

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal2-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal2-provider>
```

在此方案中，只有当你的应用作为 Web 应用程序运行并且 TeamsProvider 在当前环境中不可用时，才使用 Msal2Provider。

若要在代码中完成相同的任务，可以在提供程序上使用 `isAvailable` 属性，如下所示。

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new Msal2Provider(msalConfig)
}
```
## <a name="user-loginlogout"></a>用户登录/注销

为应用程序初始化正确的提供程序后，可以添加Toolkit[登录](../components/login.md)组件，以轻松快速地实现用户登录和注销。 该组件与提供程序一起处理所有身份验证逻辑和登录/注销功能。 以下示例使用 Msal2Provider 和 Login 组件。

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="YOUR_CLIENT_ID"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

在需要自己实现此操作（而不是使用 Toolkit 的 Login 组件）的情况下，可以使用 提供程序的 和 方法来 `login` `logout` 实现此方案。

## <a name="implement-your-own-provider"></a>实现你自己的提供程序

在想要将 Toolkit 组件添加到具有预先存在的身份验证代码的应用程序的方案中，您可以创建一个连接到身份验证机制的自定义提供程序，而不是使用预定义的提供程序。 该工具包提供两种创建新提供程序的方法：

- 创建一 `SimpleProvider` 个通过传递函数从身份验证代码返回访问令牌的新建。
- 扩展 `IProvider` 抽象类。

有关每个提供程序的更多详细信息，请参阅 [自定义提供程序](../providers/custom.md)。
