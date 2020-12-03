---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba4f6e4122a93055e2bc5a910e74850334276f59
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521486"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["{id}"]
    .Request()
    .DeleteAsync();

```