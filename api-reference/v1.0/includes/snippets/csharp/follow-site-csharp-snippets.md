---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c8f8505eda7b9d0ca73be68d61306332ca7da91d5ced2219f54cf1b5b30fa7d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378713"
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
    .Add(value)
    .Request()
    .PostAsync();

```