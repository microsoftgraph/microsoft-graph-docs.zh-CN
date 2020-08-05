---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79449ef48d09d91e0dc98c4e3f0c63d500f2ae0c
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566530"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectedOrganization = new ConnectedOrganization
{
    DisplayName = "Connected organization name",
    Description = "Connected organization description",
    IdentitySources = new List<IdentitySource>()
    {
        new DomainIdentitySource
        {
            DomainName = "example.com",
            DisplayName = "example.com"
        }
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations
    .Request()
    .AddAsync(connectedOrganization);

```