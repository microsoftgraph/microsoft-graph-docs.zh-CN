---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c3193b49b10d1336cb0a84051d782ff07624357
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795435"
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

await graphClient.Connections["{externalConnection-id}"].Items["{externalItem-id}"]
    .Request()
    .UpdateAsync(externalItem);

```