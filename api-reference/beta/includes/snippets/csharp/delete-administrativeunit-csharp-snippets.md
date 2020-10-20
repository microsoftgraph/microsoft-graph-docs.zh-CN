---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 074ce25940385710ff923c1f87555a1fef44262e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614148"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AdministrativeUnits["{id}"]
    .Request()
    .DeleteAsync();

```