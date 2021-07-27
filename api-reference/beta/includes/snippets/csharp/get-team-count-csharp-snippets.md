---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be5f88ecdfdca069ce3f1a88ee43de429e95009e
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580233"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipals = await graphClient.ServicePrincipals
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Team")
    .GetAsync();

```