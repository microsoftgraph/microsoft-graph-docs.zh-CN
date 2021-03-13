---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48da059506a0c6328b5b2fb0668666357aa3f4f3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792030"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicy = new TokenLifetimePolicy
{
    Definition = new List<String>()
    {
        "definition-value"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true
};

await graphClient.Policies.TokenLifetimePolicies["{tokenLifetimePolicy-id}"]
    .Request()
    .UpdateAsync(tokenLifetimePolicy);

```