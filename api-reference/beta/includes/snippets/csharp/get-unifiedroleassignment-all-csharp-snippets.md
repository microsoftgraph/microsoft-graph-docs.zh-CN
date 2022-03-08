---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db0a6ecd65950dec2960e5892db7d4b323ff3b9f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var transitiveRoleAssignments = await graphClient.RoleManagement.Directory.TransitiveRoleAssignments
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516'")
    .GetAsync();

```