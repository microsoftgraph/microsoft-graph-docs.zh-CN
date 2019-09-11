---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c56ba351151c38db254db55d48493a3ac04e6aa5
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845942"
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
            Id = Guid.Parse("id-value"),
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
    AppOwnerOrganizationId = Guid.Parse("appOwnerOrganizationId-value"),
    AppRoleAssignmentRequired = true
};

await graphClient.ServicePrincipals["{id}"]
    .Request()
    .UpdateAsync(servicePrincipal);

```