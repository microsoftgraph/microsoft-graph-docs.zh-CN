---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc185a1fdba510b9ddd9f0be6090d88acad74c9df6b7c13b01d3e2e461322255
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164166"
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

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"]
    .ValidateCredentials(null,null,null,credentials)
    .Request()
    .PostAsync();

```