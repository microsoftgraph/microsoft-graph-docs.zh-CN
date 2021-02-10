---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d22963f684e8f338539bc9b1daaa715eb6d2c70
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179190"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcOnPremisesConnection = await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections["{id}"]
    .Request()
    .Select("id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse")
    .GetAsync();

```