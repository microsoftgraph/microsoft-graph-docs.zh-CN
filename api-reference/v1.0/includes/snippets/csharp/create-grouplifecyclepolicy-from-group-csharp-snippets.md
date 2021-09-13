---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a669be6780354a66a92b4aa25775760820105628d2aa8869c3011b39a8ae7a2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409726"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupLifecyclePolicy = new GroupLifecyclePolicy
{
    GroupLifetimeInDays = 100,
    ManagedGroupTypes = "Selected",
    AlternateNotificationEmails = "admin@contoso.com"
};

await graphClient.GroupLifecyclePolicies
    .Request()
    .AddAsync(groupLifecyclePolicy);

```