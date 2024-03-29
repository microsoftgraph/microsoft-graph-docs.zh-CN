---
title: 自定义提供程序
description: 如果应用程序中已有身份验证代码，请创建自定义提供程序，为 Microsoft Graph Toolkit组件启用身份验证和图形访问。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 2373c30a37e761d1cd14b203aa07edfc80eecfad
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589301"
---
# <a name="custom-provider"></a>自定义提供程序

如果应用程序中已有身份验证代码，可以创建自定义提供程序，以启用 Microsoft Graph 组件的身份验证Graph Toolkit访问。 有两种方法可创建自定义提供程序：

- 通过传递 `SimpleProvider` 用于获取访问令牌的函数创建新令牌
- 扩展抽象 `IProvider` 类

本文将更详细地介绍每种方法。

## <a name="simpleprovider"></a>SimpleProvider

通过传入将 `SimpleProvider` 返回传入作用域的访问令牌的函数来实例化类。 

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

此外，还可以提供可选 `login` `logout` 和 函数，用于处理登录和从 [登录](../components/login.md) 组件注销调用。

> [!IMPORTANT] 
> 若要向组件指示他们可以在用户成功登录后开始调用 Microsoft Graph API，你需要调用 `Providers.setState(ProviderState.SignedIn)`。 以下函数中显示了这一 `login` 点的示例。

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

若要使组件了解 `provider.setState(state: ProviderState)` 提供程序的状态，则需要在状态发生更改时调用 方法。 例如，当用户登录后，调用 `provider.setState(ProviderState.SignedIn)`。 枚举 `ProviderState` 定义三种状态，如下所示。

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a>IProvider

您可以扩展抽象 `IProvider` 类以创建自己的提供程序。

### <a name="state"></a>状态

提供程序必须跟踪身份验证状态，并更新状态更改时的组件。 类 `IProvider` 已实现 `onStateChanged(eventHandler)` 处理程序和 `state: ProviderState` 属性。 只需在实现中 `setState(state:ProviderState)` 使用此方法，在状态发生更改时更新状态。 更新状态将启动事件 `stateChanged` 并自动更新所有组件。

### <a name="loginlogout"></a>登录/注销

如果提供程序提供登录或注销功能，请实现 `login(): Promise<void>` 和 `logout(): Promise<void>` 方法。 这些方法是可选的。

### <a name="access-token"></a>访问令牌

必须实现 `getAccessToken({'scopes': scopes[]}) : Promise<string>` 方法。 此方法用于获取有效的令牌之前每次调用 Microsoft Graph。

### <a name="graph"></a>Graph

这些组件使用 Microsoft Graph Javascript SDK 调用 Microsoft Graph。 提供程序必须通过 属性使 `graph` SDK 可用。 在构造函数中，创建一个新 `Graph` 实例，如下所示。

```js
this.graph = new Graph(this);
```

该类`Graph`是 Microsoft Graph SDK 顶部的浅色包装。

### <a name="example"></a>示例

所有提供程序扩展抽象 `IProvider` 类。 例如，查看任何现有提供程序的 [源代码](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/providers)。

## <a name="set-the-global-provider"></a>设置全局提供程序

组件使用 `Providers.globalProvider` 属性访问提供程序。 创建自己的提供程序后，将此属性设置为提供程序。

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

所有组件都将收到新提供程序的通知，并开始使用它。
