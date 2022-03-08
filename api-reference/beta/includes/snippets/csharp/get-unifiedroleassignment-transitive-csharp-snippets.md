---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d12936be876e34797e76bcd3608cc9cf5e51bae3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338353"
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
    .Filter("principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516' and roleDefinitionId eq 'fe930be7-5e62-47db-91af-98c3a49a38b1'")
    .GetAsync();

```