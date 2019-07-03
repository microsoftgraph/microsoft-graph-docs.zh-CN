---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 470c49291b9731789cdff260e9deb2ccf6377450
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519907"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var criteria = new SynchronizationJobRestartCriteria
{
    ResetScope = SynchronizationJobRestartScope.QuarantineState | SynchronizationJobRestartScope.Escrows | SynchronizationJobRestartScope.ConnectorDataStore
};

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"]
    .Restart(criteria)
    .Request()
    .Header("Authorization","Bearer <token>")
    .PostAsync();

```