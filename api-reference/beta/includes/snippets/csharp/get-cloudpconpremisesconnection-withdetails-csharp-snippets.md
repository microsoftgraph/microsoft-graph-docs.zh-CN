---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4628a197e24e7d9d3705e300d34320d33c5a0f61
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798104"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcOnPremisesConnection = await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections["{cloudPcOnPremisesConnection-id}"]
    .Request()
    .Select("id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse")
    .GetAsync();

```