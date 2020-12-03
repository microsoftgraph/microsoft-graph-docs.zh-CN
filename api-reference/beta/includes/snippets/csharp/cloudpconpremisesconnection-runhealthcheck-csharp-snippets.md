---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0012134da81d59fff01fb366a51844cdf089c6f2
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521640"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections["{id}"]
    .RunHealthChecks()
    .Request()
    .PostAsync();

```