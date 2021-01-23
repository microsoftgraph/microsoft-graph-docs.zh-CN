---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3eb070828c66fa28a51e7c1b6c1d65b14107be56
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945146"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cIdentityUserFlow = new B2cIdentityUserFlow
{
    Id = "Customer",
    UserFlowType = UserFlowType.SignUpOrSignIn,
    UserFlowTypeVersion = 3f,
    IdentityProviders = new B2cIdentityUserFlowIdentityProvidersCollectionPage()
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