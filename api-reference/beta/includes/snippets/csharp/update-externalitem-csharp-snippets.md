---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e36951f25dfcf05ac889e1f2ba7c58b4a5b27e6c
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47938473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalItem = new ExternalItem
{
    Acl = new List<Acl>()
    {
        new Acl
        {
            Type = AclType.User,
            Value = "49103559-feac-4575-8b94-254814dfca72",
            AccessType = AccessType.Grant,
            IdentitySource = "azureActiveDirectory"
        }
    }
};

await graphClient.Connections["contosohr"].Items["TSP228082938"]
    .Request()
    .UpdateAsync(externalItem);

```