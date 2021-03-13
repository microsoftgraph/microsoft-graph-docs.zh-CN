---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbf874c712de35a5dee82e94dec42e9bd514f01d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790263"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicy = new TokenIssuancePolicy
{
    Definition = new List<String>()
    {
        "definition-value"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true
};

await graphClient.Policies.TokenIssuancePolicies["{tokenIssuancePolicy-id}"]
    .Request()
    .UpdateAsync(tokenIssuancePolicy);

```