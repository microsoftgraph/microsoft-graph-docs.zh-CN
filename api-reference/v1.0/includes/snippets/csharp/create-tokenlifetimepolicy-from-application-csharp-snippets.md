---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f751544609d9c44614d24940d6b6b5cdb5bccd87
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806741"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicy = new TokenLifetimePolicy
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"}
    }
};

await graphClient.Applications["{id}"].TokenLifetimePolicies.References
    .Request()
    .AddAsync(tokenLifetimePolicy);

```