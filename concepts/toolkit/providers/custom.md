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
# <a name="custom-provider"></a>自定义提供程序

如果您的应用程序中有现有的身份验证代码, 则可以创建自定义提供程序, 以启用对 microsoft Graph 工具包组件的 Microsoft Graph 的身份验证和访问权限。 有两种方法可以创建自定义提供程序:

- 通过传入获取`SimpleProvider`访问令牌的函数来创建新的
- 扩展`IProvider`抽象类

本文更详细地介绍了每种方法。

## <a name="simpleprovider"></a>SimpleProvider

通过传入`SimpleProvider`将返回传入范围的访问令牌的函数来实例化类。

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

此外, 还可以提供可从[登录](../components/login.md)组件`login`处理`logout`登录和注销调用的可选和函数。

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

### <a name="manage-state"></a>管理状态

若要使组件了解提供程序的状态, 每当状态发生变化时, 都需要调用`provider.setState(state: ProviderState)`方法。 例如, 当用户登录后, 请致电`provider.setState(ProviderState.SignedIn)`。 `ProviderState`枚举定义三种状态, 如下所示。

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a>IProvider

您可以扩展`IProvider`抽象类以创建自己的提供程序。

### <a name="state"></a>状态

提供程序必须跟踪身份验证状态, 并在状态发生更改时更新组件。 `IProvider`类已实现`onStateChanged(eventHandler)`处理程序和`state: ProviderState`属性。 您只需在实现中`setState(state:ProviderState)`使用方法来更新其更改时的状态。 更新状态将触发`stateChanged`事件并自动更新所有组件。

### <a name="loginlogout"></a>登录/注销

如果提供程序提供登录或注销功能, 请实现`login(): Promise<void>`和`logout(): Promise<void>`方法。 这些方法是可选的。

### <a name="access-token"></a>访问令牌

您必须实现`getAccessToken({'scopes': scopes[]}) : Promise<string>`方法。 此方法用于在每次调用 Microsoft Graph 之前获取有效令牌。

### <a name="graph"></a>流程图

这些组件将 Microsoft Graph Javascript SDK 用于对 Microsoft Graph 的所有调用。 提供程序必须通过`graph`属性使 SDK 可用。 在构造函数中, 创建一个`Graph`新实例, 如下所示。

```js
this.graph = new Graph(this);
```

`Graph`类是 MICROSOFT Graph SDK 顶部的光包装。

### <a name="example"></a>示例

所有提供程序都扩展`IProvider`抽象类。 有关示例, 请查看任何[现有提供程序](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/src/providers)的源代码。

## <a name="set-the-global-provider"></a>设置全局提供程序

组件使用`Providers.globalProvider`属性访问提供程序。 创建自己的提供程序后, 将此属性设置为提供程序。

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

所有组件都将收到新的提供程序, 并开始使用它。
