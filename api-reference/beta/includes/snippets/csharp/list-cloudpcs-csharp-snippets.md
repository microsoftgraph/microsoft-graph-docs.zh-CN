---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 704e2adafc910f30419160d14a8e37fb5b0c4edd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522298"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPCs = await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs
    .Request()
    .GetAsync();

```