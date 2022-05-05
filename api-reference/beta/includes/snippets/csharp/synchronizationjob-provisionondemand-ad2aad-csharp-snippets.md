---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 750d7e2b4789c4309f742be6a3754885289e0411
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202892"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var parameters = new List<SynchronizationJobApplicationParameters>()
{
    new SynchronizationJobApplicationParameters
    {
        RuleId = "6c409270-f78a-4bc6-af23-7cf3ab6482fe",
        Subjects = new List<SynchronizationJobSubject>()
        {
            new SynchronizationJobSubject
            {
                ObjectId = "CN=AdeleV,CN=Users,DC=corp,DC=chicago,DC=com",
                ObjectTypeName = "user"
            }
        }
    }
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"]
    .ProvisionOnDemand(parameters)
    .Request()
    .PostAsync();

```