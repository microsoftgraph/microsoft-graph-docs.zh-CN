---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b278513d7b3919e97440ca8a96bec12271af587
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805494"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicy = new HomeRealmDiscoveryPolicy
{
    Definition = new List<String>()
    {
        "definition-value"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true
};

await graphClient.Policies.HomeRealmDiscoveryPolicies
    .Request()
    .AddAsync(homeRealmDiscoveryPolicy);

```