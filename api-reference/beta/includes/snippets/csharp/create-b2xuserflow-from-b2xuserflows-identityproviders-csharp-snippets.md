---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78636402b99abc120131a37b127963410a82683c86d8d7b19c7569a55890386d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221108"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xIdentityUserFlow = new B2xIdentityUserFlow
{
    Id = "Partner",
    UserFlowType = UserFlowType.SignUpOrSignIn,
    UserFlowTypeVersion = 1f,
    IdentityProviders = new B2xIdentityUserFlowIdentityProvidersCollectionWithReferencesPage()
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