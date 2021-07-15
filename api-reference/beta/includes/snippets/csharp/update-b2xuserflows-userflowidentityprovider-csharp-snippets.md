---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9df3ea6542f6c837e5c87a15e1248f27389e8d9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439527"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowIdentityProviders = new IdentityProviderBase
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test"}
    }
};

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].UserFlowIdentityProviders.References
    .Request()
    .UpdateAsync(userFlowIdentityProviders);

```