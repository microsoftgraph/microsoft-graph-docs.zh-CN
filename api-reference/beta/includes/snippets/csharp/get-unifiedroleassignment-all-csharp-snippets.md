---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15adb227872d12bf924b3ac97dda156d5a2714ba
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528200"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var transitiveRoleAssignments = await graphClient.RoleManagement.Directory.TransitiveRoleAssignments
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Filter("principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516'")
    .GetAsync();

```