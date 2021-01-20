---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc20841c5a80c2f7ac46300b49d3f4f5338cf680
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910646"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicy = new ClaimsMappingPolicy
{
    Definition = new List<String>()
    {
        "definition-value"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true
};

await graphClient.Policies.ClaimsMappingPolicies["{id}"]
    .Request()
    .UpdateAsync(claimsMappingPolicy);

```