---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83cb47b4616196be4984850b4c15b9639564af0d
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573164"
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
                DisplayName = "Contoso Time Manager App"
            }
        }
    }
};

await graphClient.Sites["{site-id}"].Permissions
    .Request()
    .AddAsync(permission);

```