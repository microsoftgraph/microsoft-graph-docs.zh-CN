---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29e285edd1feb87ff81b2a2d62aca87093e1d46e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439673"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowIdentityProviders = new IdentityProviderBase
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/identity/identityProviders/{id}"}
    }
};

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].UserFlowIdentityProviders.References
    .Request()
    .UpdateAsync(userFlowIdentityProviders);

```