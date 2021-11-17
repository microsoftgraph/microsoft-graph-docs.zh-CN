---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d36ef9e8c15b60751ba1e7794065129d588ea312374a59e028d3f3a80c6fc87c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161301"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicy = new TokenIssuancePolicy
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"}
    }
};

await graphClient.Applications["{application-id}"].TokenIssuancePolicies.References
    .Request()
    .AddAsync(tokenIssuancePolicy);

```