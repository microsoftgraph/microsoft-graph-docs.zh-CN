---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a353de7fda14eb24ad536f20dcc8ef823fc7da2a
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51922546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cIdentityUserFlow = new B2cIdentityUserFlow
{
    Id = "Customer",
    UserFlowType = UserFlowType.SignUpOrSignIn,
    UserFlowTypeVersion = 3f,
    IdentityProviders = new B2cIdentityUserFlowIdentityProvidersCollectionWithReferencesPage()
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