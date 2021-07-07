---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 673a272f923528117aa1f125ee3ff4be4c490ab6
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316971"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAuditActivityTypes = await graphClient.DeviceManagement.VirtualEndpoint.AuditEvents
    .GetAuditActivityTypes()
    .Request()
    .GetAsync();

```