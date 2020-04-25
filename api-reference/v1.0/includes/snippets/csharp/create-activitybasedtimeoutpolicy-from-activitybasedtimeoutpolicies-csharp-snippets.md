---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 378799397d74071dc2a129fc92da87cee4649d63
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806298"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activityBasedTimeoutPolicy = new ActivityBasedTimeoutPolicy
{
    Definition = new List<String>()
    {
        "definition-value"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true
};

await graphClient.Policies.ActivityBasedTimeoutPolicies
    .Request()
    .AddAsync(activityBasedTimeoutPolicy);

```