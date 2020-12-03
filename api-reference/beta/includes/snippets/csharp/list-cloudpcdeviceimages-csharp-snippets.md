---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b847e45f5baa11aebbeab9c42023107705a529e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522442"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deviceImages = await graphClient.DeviceManagement.VirtualEndpoint.DeviceImages
    .Request()
    .GetAsync();

```