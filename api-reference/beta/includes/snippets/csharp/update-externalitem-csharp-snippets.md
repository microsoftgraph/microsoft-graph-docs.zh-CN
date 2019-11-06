---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0758f028431ad857e8463bcd52d867beac2b6392
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994483"
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
            IdentitySource = "Azure Active Directory"
        }
    }
};

await graphClient.Connections["contosohr"].Items["TSP228082938"]
    .Request()
    .UpdateAsync(externalItem);

```