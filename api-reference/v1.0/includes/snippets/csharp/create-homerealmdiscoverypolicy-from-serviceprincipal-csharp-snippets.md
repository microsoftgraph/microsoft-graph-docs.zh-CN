---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdc7e19c5e2689de4a0b7906b88713e9f5ebb5d720fc3e685e1c84a02a79d6b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicy = new HomeRealmDiscoveryPolicy
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"}
    }
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].HomeRealmDiscoveryPolicies.References
    .Request()
    .AddAsync(homeRealmDiscoveryPolicy);

```