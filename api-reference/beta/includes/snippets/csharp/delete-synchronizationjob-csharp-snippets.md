---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6a6799fb161d323504e858e272859e310fd5ede6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479277"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"]
    .Request()
    .DeleteAsync();

```