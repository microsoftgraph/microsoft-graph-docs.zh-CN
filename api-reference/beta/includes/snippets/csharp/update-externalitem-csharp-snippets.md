---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58958bb80aa4a710a037a46d7724ea7388d363fc
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48230749"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalItem = new ExternalItem
{
    Acl = new List<Acl>()
    {
        new Acl
        {
            Type = AclType.Everyone,
            Value = "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
            AccessType = AccessType.Grant,
            IdentitySource = "azureActiveDirectory"
        }
    }
};

await graphClient.Connections["contosohr"].Items["TSP228082938"]
    .Request()
    .UpdateAsync(externalItem);

```