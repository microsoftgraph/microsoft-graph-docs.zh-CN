---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 194aec85f4ca1704bab0e1c19ba52de4d0a4b89c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614784"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<Site>()
{
    new Site
    {
        Id = "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740"
    },
    new Site
    {
        Id = "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851"
    }
};

await graphClient.Users["{user-id}"].FollowedSites
    .Remove(value)
    .Request()
    .PostAsync();

```