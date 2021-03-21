---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4b92be366e588669607b7067fe2caa7a3622bcd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956728"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryAudit = await graphClient.AuditLogs.DirectoryAudits["{directoryAudit-id}"]
    .Request()
    .GetAsync();

```