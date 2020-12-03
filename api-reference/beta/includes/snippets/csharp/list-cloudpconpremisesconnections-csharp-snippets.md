---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b51a741dfe0dc263ce9a56508ff28fd81f47ee44
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522625"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onPremisesConnections = await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections
    .Request()
    .GetAsync();

```