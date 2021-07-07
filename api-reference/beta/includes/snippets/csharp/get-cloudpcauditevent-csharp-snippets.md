---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 344c13af06e9bc2d4341ba4121432a458df0f54e
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316880"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcAuditEvent = await graphClient.DeviceManagement.VirtualEndpoint.AuditEvents["{cloudPcAuditEvent-id}"]
    .Request()
    .GetAsync();

```