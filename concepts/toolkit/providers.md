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
# <a name="microsoft-graph-toolkit-providers"></a>Microsoft Graph 工具包提供程序

Microsoft Graph 工具包提供程序使应用程序能够使用 Microsoft Identity 进行身份验证，并在仅几行代码中访问 Microsoft Graph。 每个提供程序处理用户身份验证并获取访问令牌以调用 Microsoft Graph Api，因此您无需自己编写此代码。 

您可以使用自己的提供程序（不含组件）快速为您的应用程序实现身份验证，并通过 JavaScript 客户端 SDK 调用 Microsoft Graph。

使用 Microsoft Graph 工具包组件时，这些提供程序是必需的，因为组件使用它们来访问 Microsoft Graph。 如果您已经有自己的身份验证并且想要使用组件，则可以改为使用 [自定义提供程序](./providers/custom.md) 。

该工具包包括以下提供程序。

|提供程序|说明|
|---------|-----------|
|[Msal](./providers/msal.md)|使用 MSAL.js 在 web 应用程序中登录用户和获取令牌以与 Microsoft Graph 一起使用。|
|[SharePoint](./providers/sharepoint.md)|对 SharePoint web 部件内的组件进行身份验证并提供 Microsoft Graph 访问权限。|
|[Teams](./providers/teams.md)|对 Microsoft 团队选项卡中的组件进行身份验证和提供 Microsoft Graph 访问。|
|[代理](./providers/proxy.md)|通过将对 Microsoft Graph 的所有调用通过后端路由，允许使用后端身份验证。|
|[自定义](./providers/custom.md)|创建自定义提供程序，以便通过应用程序的现有身份验证代码启用对 Microsoft Graph 的身份验证和访问。|

## <a name="initializing-a-provider"></a>初始化提供程序

若要在应用程序中使用提供程序，您需要初始化一个新的提供程序，然后将其设置为 provider 命名空间中的全局提供程序。 我们建议您在开始使用任何组件之前执行此操作。 可以通过以下两种方式之一执行此操作：

**选项1：使用提供程序组件**

您可以直接在 HTML 中使用提供程序的组件版本。 在幕后，将初始化新的提供程序并将其设置为全局提供程序。 下面的示例演示如何使用 MsalProvider。

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

**选项2：在代码中初始化**

通过在 JavaScript 代码中初始化提供程序，可以提供更多的选项。 为此，请创建一个新的提供程序实例，并将该属性的值设置 `Providers.globalProvider` 为您想要使用的提供程序。 下面的示例演示如何使用 MsalProvider。

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> **注意：** 有关如何注册您的应用程序并获取客户端 ID 的详细信息，请参阅 [Create a Azure Active Directory app](./get-started/add-aad-app-registration.md)。

## <a name="permission-scopes"></a>权限范围

建议在初始化提供程序时添加应用程序需要的所有权限范围， `scopes` (此属性不应用于 [SharePoint 提供程序](./providers/sharepoint.md)) 。 这是可选的，但将通过向用户提供应用程序中所有组件请求的权限的聚合列表，而不是为每个组件呈现单独的屏幕，来改善用户体验。 下面的示例演示如何使用 MsalProvider 执行此操作。

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

如果要在代码中初始化提供程序，请在属性中提供数组中的权限范围 `scopes` 。

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

可以在每个组件的 "文档" 页的 " **Microsoft Graph 权限** " 一节中找到每个组件所需的权限范围列表。

## <a name="provider-state"></a>提供程序状态

提供程序跟踪用户的身份验证状态并将其传递到组件。 例如，当用户成功登录时，将 `ProviderState` 更新为 `SignedIn` ，向这些组件发出信号，通知他们现在可以调用 Microsoft Graph。 `ProviderState`枚举定义三种状态，如下所示。

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

在某些情况下，您可能需要显示特定功能或仅在用户成功登录后执行某项操作。 您可以访问和检查提供程序状态，如下面的示例所示。

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
您还可以使用 `Providers.onProviderUpdated` 方法在提供程序的状态更改时收到通知。

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

每个提供程序公开一个调用 `getAccessToken` 的函数，该函数可以检索当前访问令牌或检索提供的作用域的新访问令牌。 下面的示例演示如何获取具有权限范围的新访问令牌 `User.Read` 。

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = Provider.globalProvider.getAccessToken({scopes: 'User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a>对 Microsoft Graph 进行自己的调用

所有组件都可以访问 Microsoft Graph，而无需进行任何自定义，只要您初始化提供程序 (如上一节) 中所述。 如果要对 Microsoft Graph 进行自己的调用，可以通过获取对组件使用的相同 Microsoft Graph SDK 的引用来执行此操作。 首先，获取对全局的引用 `IProvider` ，然后按 `graph` 如下所示使用对象：

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
在某些情况下，您可能需要传递其他权限，具体取决于您要调用的 API。 以下示例说明了具体的操作方法。

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a>使用多个提供程序

在某些情况下，您的应用程序将在不同的环境中运行，每个都需要不同的提供程序。 例如，应用程序可能同时作为 web 应用程序和 Microsoft 团队选项卡运行，这意味着您可能需要同时使用 MsalProvider 和 TeamsProvider。 对于此方案，所有提供程序组件都具有 `depends-on` 创建回退链的属性，如下面的示例所示。

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

在这种情况下，仅当应用程序作为 web 应用程序运行，并且 TeamsProvider 在当前环境中不可用时，才会使用 MsalProvider。

若要在代码中实现相同，可以使用 `isAvailable` 提供程序上的属性，如下所示。

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```
## <a name="user-loginlogout"></a>用户登录/注销

如果为应用程序初始化了正确的提供程序，则可以添加该工具包的 [登录组件](./components/login.md) ，以便轻松快速地实现用户登录和注销。 组件与提供程序配合使用，以处理所有身份验证逻辑和登录/注销功能。 下面的示例使用 MsalProvider 和 Login 组件。

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
<mgt-login></mgt-login>
```

在您希望自己实现这一点的方案中，您可以使用 `login` 提供程序的和方法来执行此操作，而不是使用该工具包的登录组件 `logout` 。

## <a name="implement-your-own-provider"></a>实现您自己的提供程序

在要将工具包组件添加到具有预先存在的身份验证代码的应用程序的方案中，您可以创建一个挂接到您的身份验证机制中的自定义提供程序，而不是使用预定义的提供程序。 该工具包提供了两种创建新的提供程序的方法：

- 创建一个新 `SimpleProvider` 的，它通过传入函数返回身份验证代码中的访问令牌。
- 扩展 `IProvider` 抽象类。

有关每个的详细信息，请参阅 [自定义提供程序](./providers/custom.md)。
