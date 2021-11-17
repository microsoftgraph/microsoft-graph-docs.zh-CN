---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcba191b3e1a3c02dbd63e986416781287684388fc5fb70c10b83ae694b8cfb6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902600"
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