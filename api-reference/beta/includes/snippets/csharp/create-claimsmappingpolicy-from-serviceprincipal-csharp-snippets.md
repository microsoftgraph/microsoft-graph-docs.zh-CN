---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bf73ccfead99bd5e01326414cb5780550e5c7c4e80c77011c9ed0bf600e07eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220779"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicy = new ClaimsMappingPolicy
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"}
    }
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].ClaimsMappingPolicies.References
    .Request()
    .AddAsync(claimsMappingPolicy);

```