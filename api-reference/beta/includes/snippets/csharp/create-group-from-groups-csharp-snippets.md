---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ffb5ff06a20c7528f0612fa389d4dcd027469a3
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780507"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/odata/groups('1a9db3ab-0acf-4808-99ae-e8ed581cb2e0')"}
    }
};

await graphClient.Policies.MobileAppManagementPolicies["{mobilityManagementPolicy-id}"].IncludedGroups.References
    .Request()
    .AddAsync(group);

```