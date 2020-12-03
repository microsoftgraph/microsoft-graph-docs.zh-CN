---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71dd01dd9fc39862fbe4494e9af97f5110973598
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521941"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPC = await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["{id}"]
    .Request()
    .GetAsync();

```