---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 792e55094385abeef6c96d79cd47e63ce2278a92
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797251"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections["{cloudPcOnPremisesConnection-id}"]
    .RunHealthChecks()
    .Request()
    .PostAsync();

```