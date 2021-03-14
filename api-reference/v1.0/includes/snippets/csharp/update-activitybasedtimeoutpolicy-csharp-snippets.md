---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ace2992316f6704e6fd4cad91e9dacb6ad4a135
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789671"
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

await graphClient.Policies.ActivityBasedTimeoutPolicies["{activityBasedTimeoutPolicy-id}"]
    .Request()
    .UpdateAsync(activityBasedTimeoutPolicy);

```