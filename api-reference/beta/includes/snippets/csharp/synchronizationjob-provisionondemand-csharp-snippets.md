---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14e96df1875a5c3f08c3158d6632d8ca7e1f7da5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809697"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var parameters = new List<SynchronizationJobApplicationParameters>()
{
    new SynchronizationJobApplicationParameters
    {
        Subjects = new List<SynchronizationJobSubject>()
        {
            new SynchronizationJobSubject
            {
                ObjectId = "9bb0f679-a883-4a6f-8260-35b491b8b8c8",
                ObjectTypeName = "User"
            }
        },
        RuleId = "ea807875-5618-4f0a-9125-0b46a05298ca"
    }
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"]
    .ProvisionOnDemand(parameters)
    .Request()
    .PostAsync();

```