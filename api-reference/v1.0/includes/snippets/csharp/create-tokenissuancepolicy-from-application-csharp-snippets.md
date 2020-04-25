---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56250dbef3410f8e24204b14bca9aaf4ef8f4b1d
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806812"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicy = new TokenIssuancePolicy
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"}
    }
};

await graphClient.Applications["{id}"].TokenIssuancePolicies.References
    .Request()
    .AddAsync(tokenIssuancePolicy);

```