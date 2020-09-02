---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad48f4b67056d591b006b9254a0d665a96da3c33
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329975"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cIdentityUserFlow = new B2cIdentityUserFlow
{
    Id = "Customer",
    UserFlowType = UserFlowType.SignUpOrSignIn,
    UserFlowTypeVersion = 3f,
    IdentityProviders = (IB2cIdentityUserFlowIdentityProvidersCollectionPage)new List<IdentityProvider>()
    {
        new IdentityProvider
        {
            Id = "Facebook-OAuth",
            Type = "Facebook",
            Name = "Facebook"
        }
    }
};

await graphClient.Identity.B2cUserFlows
    .Request()
    .AddAsync(b2cIdentityUserFlow);

```