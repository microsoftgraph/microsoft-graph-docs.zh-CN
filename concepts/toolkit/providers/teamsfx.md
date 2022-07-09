---
title: TeamsFx 提供商
description: 使用 Microsoft Teams 应用程序中的 TeamsFx 提供程序为 Microsoft Graph 工具包组件提供对 Microsoft Graph 的访问权限。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: f5a94ab3fc133ebe38ec552ae152b182000311f7
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698399"
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
// Put this code in a call-to-action callback function to avoid browser blocking automatically showing up pop-ups. 
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

有关演示如何初始化 TeamsFx 提供程序的示例，请参阅 [联系人导出程序示例](https://github.com/OfficeDev/TeamsFx-Samples/tree/dev/hello-world-tab-with-backend)。


## <a name="see-also"></a>另请参阅
* [Microsoft Teams 和 Teams 工具包开发入门](https://aka.ms/teamsfx-docs)
* [TeamsFx SDK](/microsoftteams/platform/toolkit/teamsfx-sdk)
* [一个生产力中心研讨会](https://github.com/OfficeDev/OneProductivityHub-TeamsFx)
