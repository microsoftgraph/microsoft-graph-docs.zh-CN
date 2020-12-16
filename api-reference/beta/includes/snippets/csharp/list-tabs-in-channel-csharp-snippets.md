---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58a99d2537f2b6356b3bfb5f2359b9fca2d9549e
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690132"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tabs = await graphClient.Teams["6903fa93-605b-43ef-920e-77c4729f8258"].Channels["19:33b76eea88574bd1969dca37e2b7a819@thread.skype"].Tabs
    .Request()
    .Expand("teamsApp")
    .GetAsync();

```