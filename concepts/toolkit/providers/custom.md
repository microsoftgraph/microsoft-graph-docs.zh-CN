---
title: 自定义提供程序
description: 如果您的应用程序中有现有的身份验证代码，则创建自定义提供程序以启用 Microsoft Graph 工具包组件的身份验证和图形访问。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 57b7ca843f71d22992df18dc2466d0182d3fc556
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086597"
---
# <a name="custom-provider"></a>自定义提供程序

如果您的应用程序中有现有的身份验证代码，则可以创建自定义提供程序，以启用对 microsoft Graph 工具包组件的 Microsoft Graph 的身份验证和访问权限。 有两种方法可以创建自定义提供程序：

- `SimpleProvider`通过传入获取访问令牌的函数来创建新的
- 扩展 `IProvider` 抽象类

本文更详细地介绍了每种方法。

## <a name="simpleprovider"></a>SimpleProvider

`SimpleProvider`通过传入将返回传入范围的访问令牌的函数来实例化类。 

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

此外，还可以提供 `login` `logout` 可从 [登录](../components/login.md) 组件处理登录和注销调用的可选和函数。

> [!IMPORTANT] 
> 若要指示用户在成功登录后可以开始调用 Microsoft Graph Api 的组件，您需要调用 `Providers.setState(ProviderState.SignedIn)` 。 下面的函数中显示了这一示例 `login` 。

```ts
function getAccessToken(scopes: string[]) {
  // return a promise with accessToken string
}

function login() {
  //login code
  Providers.globalProvider.setState(ProviderState.SignedIn)
}

function logout() {
  // logout code
}

let provider = new SimpleProvider(getAccessToken, login, logout);
```

### <a name="manage-state"></a>管理状态

若要使组件了解提供程序的状态， `provider.setState(state: ProviderState)` 每当状态发生变化时，都需要调用方法。 例如，当用户登录后，请致电 `provider.setState(ProviderState.SignedIn)` 。 `ProviderState`枚举定义三种状态，如下所示。

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a>IProvider

您可以扩展 `IProvider` 抽象类以创建自己的提供程序。

### <a name="state"></a>状态

提供程序必须跟踪身份验证状态，并在状态发生更改时更新组件。 `IProvider`类已实现 `onStateChanged(eventHandler)` 处理程序和 `state: ProviderState` 属性。 您只需在 `setState(state:ProviderState)` 实现中使用方法来更新其更改时的状态。 更新状态将触发 `stateChanged` 事件并自动更新所有组件。

### <a name="loginlogout"></a>登录/注销

如果提供程序提供登录或注销功能，请实现 `login(): Promise<void>` 和 `logout(): Promise<void>` 方法。 这些方法是可选的。

### <a name="access-token"></a>访问令牌

您必须实现 `getAccessToken({'scopes': scopes[]}) : Promise<string>` 方法。 此方法用于在每次调用 Microsoft Graph 之前获取有效令牌。

### <a name="graph"></a>Graph

这些组件将 Microsoft Graph Javascript SDK 用于对 Microsoft Graph 的所有调用。 提供程序必须通过属性使 SDK 可用 `graph` 。 在构造函数中，创建一个新 `Graph` 实例，如下所示。

```js
this.graph = new Graph(this);
```

`Graph`类是 Microsoft GRAPH SDK 顶部的光包装。

### <a name="example"></a>示例

所有提供程序都扩展 `IProvider` 抽象类。 有关示例，请查看任何 [现有提供程序](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/mgt/src/providers)的源代码。

## <a name="set-the-global-provider"></a>设置全局提供程序

组件使用 `Providers.globalProvider` 属性访问提供程序。 创建自己的提供程序后，将此属性设置为提供程序。

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

所有组件都将收到新的提供程序，并开始使用它。
