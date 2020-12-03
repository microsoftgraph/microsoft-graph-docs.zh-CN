---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d698749bc59d3c9178a7ed2ab4806cb262a42241
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521808"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcDeviceImage = await graphClient.DeviceManagement.VirtualEndpoint.DeviceImages["{id}"]
    .Request()
    .GetAsync();

```