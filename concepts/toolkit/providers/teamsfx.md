---
title: TeamsFx 提供程序
description: 使用Microsoft Teams应用程序中的 TeamsFx 提供程序为 Microsoft Graph Toolkit 组件提供对 Microsoft Graph 的访问权限。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 62df3d038c7a407da77e92b1d4de04fd1832aacf
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694390"
---
# <a name="teamsfx-provider"></a>TeamsFx 提供程序

使用Microsoft Teams应用程序中的 TeamsFx 提供程序为 Microsoft Graph Toolkit 组件提供对 Microsoft Graph 的访问权限。

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
* [开始Microsoft Teams和Teams Toolkit开发](https://aka.ms/teamsfx-docs)
