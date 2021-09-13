---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35642d8a83f283f72d6c3a6c909d9f77aff34e97687be4b7ed83d5033adbfcf1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220205"
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