---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c43be70b95b2beaa466ecb7e8664380b16dead5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956692"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryAudits = await graphClient.AuditLogs.DirectoryAudits
    .Request()
    .GetAsync();

```