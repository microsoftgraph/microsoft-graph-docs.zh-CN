---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4b71da7daaa8b6c239f00048adbe720e394f6f95e5e8bae588b3790934c33bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219889"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tabs = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Tabs
    .Request()
    .Filter("teamsApp/id eq 'com.microsoft.teamspace.tab.planner'")
    .Expand("teamsApp")
    .GetAsync();

```