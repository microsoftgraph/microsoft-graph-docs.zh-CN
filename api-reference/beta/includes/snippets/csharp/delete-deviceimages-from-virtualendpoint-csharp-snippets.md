---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 729a265343cd9454e19aa44e70f34aa0b0d433b5
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521892"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.DeviceImages["{id}"]
    .Request()
    .DeleteAsync();

```