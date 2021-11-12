---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ffd660d3982a9794cd331fd29f34c144d6ee4467d9d98cbb7cfaf54b4de34a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161573"
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
    },
    State = ConnectedOrganizationState.Proposed
};

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations
    .Request()
    .AddAsync(connectedOrganization);

```