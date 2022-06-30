---
title: TeamsFx 提供商
description: 使用 Microsoft Teams 应用程序中的 TeamsFx 提供程序为 Microsoft Graph 工具包组件提供对 Microsoft Graph 的访问权限。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 0789bcff15b523ae8227a2dccf3b0360810fd64e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438239"
---
# <a name="teamsfx-provider"></a>TeamsFx 提供商

使用 Microsoft Teams 应用程序中的 TeamsFx 提供程序为 Microsoft Graph 工具包组件提供对 Microsoft Graph 的访问权限。

若要详细了解身份验证提供程序，请参阅 [提供程序](./providers.md)。

## <a name="get-started"></a>入门

在组件中初始化提供程序。

```ts
// Import the providers and credential at the top of the page
import {Providers} from '@microsoft/mgt-element';
import {TeamsFxProvider} from '@microsoft/mgt-teamsfx-provider';
import {TeamsUserCredential} from "@microsoft/teamsfx";

const scope = ["User.Read"];
const teamsfx = new TeamsFx();
const provider = new TeamsFxProvider(teamsfx, scope);
Providers.globalProvider = provider;
```

使用该 `teamsfx.login(scopes)` 方法获取所需的访问令牌。

```ts
// Automatically when loading the component or in a call-to-action
await teamsfx.login(this.scope);
Providers.globalProvider.setState(ProviderState.SignedIn);
```

现在，在使用 React 时，可以在 HTML 页面或方法中`render()`添加任何组件，并使用 TeamsFx 上下文访问 Microsoft Graph。

```html
<!-- Using HTML -->
<mgt-person query="me" view="threeLines"></mgt-person>
```

```ts
// Using React
public render(): void {
  return (
      <div>
        <Person personQuery="me" view={PersonViewType.threelines}></Person>
      </div>
  );
}
```

有关演示如何初始化 TeamsFx 提供程序的示例，请参阅 [联系人导出程序示例](https://github.com/OfficeDev/TeamsFx-Samples/tree/ga/graph-toolkit-contact-exporter)。


## <a name="see-also"></a>另请参阅
* [Microsoft Teams 和 Teams 工具包开发入门](https://aka.ms/teamsfx-docs)
* [一个生产力中心研讨会](https://github.com/OfficeDev/OneProductivityHub-TeamsFx)
