---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1193daaf5dc8fbabb1000952d3b2ba15a0ffed6c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500677"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Resume()
    .Request()
    .PostAsync();

```