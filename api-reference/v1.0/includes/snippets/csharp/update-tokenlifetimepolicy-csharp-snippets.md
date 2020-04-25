---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d7427ff6090c783ff42a35c115fcaf00f7055c0
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806024"
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
    IsOrganizationDefault = true,
    Type = "type-value"
};

await graphClient.Policies.TokenLifetimePolicies["{id}"]
    .Request()
    .UpdateAsync(tokenLifetimePolicy);

```