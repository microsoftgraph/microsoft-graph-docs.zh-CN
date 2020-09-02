---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 996618fcb6cdb8298f6d94c5b90de056361ff7ea
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329588"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xIdentityUserFlow = new B2xIdentityUserFlow
{
    Id = "Partner",
    UserFlowType = UserFlowType.SignUpOrSignIn,
    UserFlowTypeVersion = 1f,
    IdentityProviders = (IB2xIdentityUserFlowIdentityProvidersCollectionPage)new List<IdentityProvider>()
    {
        new IdentityProvider
        {
            Id = "Facebook-OAuth",
            Type = "Facebook",
            Name = "Facebook"
        }
    }
};

await graphClient.Identity.B2xUserFlows
    .Request()
    .AddAsync(b2xIdentityUserFlow);

```