---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 022d151d2db87c4b7c809749ad1a56a0b7e4dae5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775073"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var criteria = new SynchronizationJobRestartCriteria
{
    ResetScope = SynchronizationJobRestartScope.Escrows | SynchronizationJobRestartScope.Watermark | SynchronizationJobRestartScope.QuarantineState
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"]
    .Restart(criteria)
    .Request()
    .Header("Authorization","Bearer <token>")
    .PostAsync();

```