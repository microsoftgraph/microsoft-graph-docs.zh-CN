---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a5a2dec1d6f149849612670e63f60601b122b1d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60690145"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appManagementPolicy = new AppManagementPolicy
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}"}
    }
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppManagementPolicies.References
    .Request()
    .AddAsync(appManagementPolicy);

```