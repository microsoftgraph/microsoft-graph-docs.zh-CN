---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5259b72e24baba4966735b5f0711beb560414dca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795593"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permission = new Permission
{
    Roles = new List<String>()
    {
        "write"
    },
    GrantedToIdentities = new List<IdentitySet>()
    {
        new IdentitySet
        {
            Application = new Identity
            {
                Id = "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
                DisplayName = "Foo App"
            }
        }
    }
};

await graphClient.Sites["{site-id}"].Permissions
    .Request()
    .AddAsync(permission);

```