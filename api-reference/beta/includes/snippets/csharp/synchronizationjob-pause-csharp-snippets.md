---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9572bdc7745cff5bb0c4e824018dc90685f3ecf8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725016"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"]
    .Pause()
    .Request()
    .PostAsync();

```