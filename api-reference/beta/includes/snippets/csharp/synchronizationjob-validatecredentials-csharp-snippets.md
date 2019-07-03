---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a127300a62f908ab73226610dfd695e330617cbd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519905"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentials = new List<SynchronizationSecretKeyStringValuePair>()
{
    new SynchronizationSecretKeyStringValuePair
    {
        Key = SynchronizationSecret.UserName,
        Value = "user@domain.com"
    },
    new SynchronizationSecretKeyStringValuePair
    {
        Key = SynchronizationSecret.Password,
        Value = "password-value"
    }
};

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{id}"]
    .ValidateCredentials(applicationIdentifier,templateId,useSavedCredentials,credentials)
    .Request()
    .PostAsync();

```