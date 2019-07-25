---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8100bab2ceddc26d7de500220eff81ea2ec13b89
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725226"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = new ServicePrincipal
{
    AccountEnabled = true,
    AddIns = new List<AddIn>()
    {
        new AddIn
        {
            Id = "id-value",
            Type = "type-value",
            Properties = new List<KeyValue>()
            {
                new KeyValue
                {
                    Key = "key-value",
                    Value = "value-value"
                }
            }
        }
    },
    AppDisplayName = "appDisplayName-value",
    AppId = "appId-value",
    AppOwnerOrganizationId = "appOwnerOrganizationId-value",
    AppRoleAssignmentRequired = true
};

await graphClient.ServicePrincipals["{id}"]
    .Request()
    .UpdateAsync(servicePrincipal);

```