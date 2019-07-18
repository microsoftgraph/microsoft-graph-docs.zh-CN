---
title: Microsoft Graph 工具包提供程序
description: Microsoft Graph 工具包提供程序为所有组件启用身份验证和 Microsoft Graph 访问。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 3e5d587e8c2690d2b71a2e70e41266519566f91e
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778710"
---
# <a name="microsoft-graph-toolkit-providers"></a>Microsoft Graph 工具包提供程序

Microsoft Graph 工具包提供程序为所有组件启用身份验证和 Microsoft Graph 访问。 每个提供程序都提供用于获取调用 Microsoft Graph Api 所需的访问令牌的实现。

对于要使用提供程序的组件, 必须将该`Providers.globalProvider`属性设置为要使用的提供程序的值。

下面的示例演示如何使用 MsalProvider。

```js
Providers.globalProvider = new MsalProvider({
  clientId: '[CLIENT_ID]'
});
```

此工具包实现以下提供程序:

- [MsalProvider](./providers/msal.md)
- [SharePointProvider](./providers/sharepoint.md)
- [TeamsProvider](./providers/teams.md)
- Office 外接程序提供程序 (即将推出)

## <a name="get-started"></a>入门

您可以随时创建提供程序。 我们建议您先创建提供程序, 然后再使用任何组件。 本节介绍如何初始化提供程序。

`Providers`全局变量公开以下属性和函数

- `globalProvider : IProvider`

将此属性设置为要全局使用的提供程序。 所有组件均使用此属性获取对提供程序的引用。 设置此属性将触发该`onProvidersChanged`事件。

- `function onProviderUpdated(callbackFunction)`

当`callbackFunction`提供程序发生更改或提供程序的状态更改时, 将调用此函数。 `ProvidersChangedState`枚举值将传递给函数以指示更新的内容。

## <a name="implement-your-own-provider"></a>实现您自己的提供程序

该工具包提供了两种创建新的提供程序的方法:

- 通过传入获取`SimpleProvider`访问令牌的函数来创建新的
- 扩展`IProvider`抽象类

有关详细信息, 请参阅[自定义提供程序](./providers/custom.md)文档中的每一个。

## <a name="making-your-own-calls-to-microsoft-graph"></a>对 Microsoft Graph 进行自己的调用

只要您初始化提供程序 (如上一节中所述), 所有组件都可以访问 Microsoft Graph, 而无需进行任何自定义。 若要获取对组件使用的同一 Microsoft Graph SDK 的引用, 请首先获取对全局 IProvider 的引用, 然后使用该`Graph`对象, 如图所示。

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```

在某些情况下, 您可能需要传递其他权限, 具体取决于您要调用的 API。

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

该`graph`对象是[MICROSOFT graph Javascript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript)的一个实例, 可以使用它对 microsoft graph 进行任何调用。
