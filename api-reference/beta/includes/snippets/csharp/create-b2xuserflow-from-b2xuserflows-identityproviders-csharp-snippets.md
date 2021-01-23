---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5bca844aeeb3406ed85b6962aed28b402270c52
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946088"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xIdentityUserFlow = new B2xIdentityUserFlow
{
    Id = "Partner",
    UserFlowType = UserFlowType.SignUpOrSignIn,
    UserFlowTypeVersion = 1f,
    IdentityProviders = new B2xIdentityUserFlowIdentityProvidersCollectionPage()
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