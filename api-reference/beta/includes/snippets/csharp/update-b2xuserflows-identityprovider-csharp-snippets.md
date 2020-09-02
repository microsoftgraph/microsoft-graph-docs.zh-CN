---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44b8a1c442a2796b47564cea46245a1f6f3c004e
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329498"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = new IdentityProvider
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/identityProviders/{id}"}
    }
};

await graphClient.Identity.B2xUserFlows["{id}"].IdentityProviders.References
    .Request()
    .UpdateAsync(identityProviders);

```