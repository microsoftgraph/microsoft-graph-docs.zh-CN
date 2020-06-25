---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73a44fc84ff6f5d1b6f340796379935fbf3b2f9e
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863231"
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

await graphClient.Policies.ClaimsMappingPolicies
    .Request()
    .AddAsync(claimsMappingPolicy);

```