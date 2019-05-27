---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 074ce25940385710ff923c1f87555a1fef44262e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439139"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AdministrativeUnits["{id}"]
    .Request()
    .DeleteAsync();

```