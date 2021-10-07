---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf8d22b27b109b533a5809689b3761f45d01c548
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214786"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAllMessages = await graphClient.Teams["{team-id}"].Channels
    .GetAllMessages()
    .Request()
    .Filter("lastModifiedDateTime gt 2019-11-01T00:00:00Z and lastModifiedDateTime lt 2021-11-01T00:00:00Z")
    .GetAsync();

```