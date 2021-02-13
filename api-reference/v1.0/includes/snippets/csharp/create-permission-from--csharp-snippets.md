---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33deb9c708cd270361a155ce37d52335910b1173
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176771"
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

await graphClient.Sites["{sitesId}"].Permissions
    .Request()
    .AddAsync(permission);

```