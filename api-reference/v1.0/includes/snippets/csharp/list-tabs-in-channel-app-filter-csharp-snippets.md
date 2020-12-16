---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84cb73794a971bd200a262783f84b24a577bf235
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690461"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tabs = await graphClient.Teams["6903fa93-605b-43ef-920e-77c4729f8258"].Channels["19:33b76eea88574bd1969dca37e2b7a819@thread.skype"].Tabs
    .Request()
    .Filter("teamsApp/id eq 'com.microsoft.teamspace.tab.planner'")
    .Expand("teamsApp")
    .GetAsync();

```