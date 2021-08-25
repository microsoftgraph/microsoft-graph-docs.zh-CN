---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d330b938f151b026d5e26cd9b369973f53f6681fd4fad7a58470e5adabe01f94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePlanId = Guid.Parse("28f42d6f-8034-4a0f-9d8a-a218a63b3299");

var skuId = Guid.Parse("465a2a90-5e59-456d-a7b8-127b9fb2e484");

await graphClient.Me
    .ActivateServicePlan(servicePlanId,skuId)
    .Request()
    .PostAsync();

```