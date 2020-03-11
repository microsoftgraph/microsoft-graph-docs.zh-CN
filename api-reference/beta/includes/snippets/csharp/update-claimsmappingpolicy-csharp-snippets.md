---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47a525fe75200603d63d2c04acb2044756c2c266
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589681"
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
    IsOrganizationDefault = true,
    Type = "type-value"
};

await graphClient.Policies.ClaimsMappingPolicies["{id}"]
    .Request()
    .UpdateAsync(claimsMappingPolicy);

```