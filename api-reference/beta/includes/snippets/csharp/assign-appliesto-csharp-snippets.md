---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e793094d848c492f4f96c37fe044e905d867c4cd
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262498"
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

await graphClient.Applications["{application-id}"].AppManagementPolicies.References
    .Request()
    .AddAsync(appManagementPolicy);

```