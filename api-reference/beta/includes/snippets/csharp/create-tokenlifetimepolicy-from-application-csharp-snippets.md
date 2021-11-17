---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0aa6670630bc042c762e275001acacca733ff2a2a8ede7e2aecd9e39895e11bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161304"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicy = new TokenLifetimePolicy
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"}
    }
};

await graphClient.Applications["{application-id}"].TokenLifetimePolicies
    .Request()
    .AddAsync(tokenLifetimePolicy);

```