---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9572bdc7745cff5bb0c4e824018dc90685f3ecf8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466019"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"]
    .Pause()
    .Request()
    .PostAsync();

```