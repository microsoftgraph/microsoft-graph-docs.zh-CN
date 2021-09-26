---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bc9077531fd562f270d438d35972ec337501c89
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763494"
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
            Id = "Facebook-OAuth"
        }
    }
};

await graphClient.Identity.B2cUserFlows
    .Request()
    .Header("Location","https://graph.microsoft.com/beta/identity/b2cUserFlows('B2C_1_Customer')")
    .AddAsync(b2cIdentityUserFlow);

```