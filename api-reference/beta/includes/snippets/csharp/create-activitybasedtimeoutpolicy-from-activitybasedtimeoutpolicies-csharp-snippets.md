---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e34b8ed892885c0dba32979b76f67369329c52ac708c5d23844654b9729f0796
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902603"
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