---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f85d6d14e8f592c455c6eaf58e84dc34b5289d5
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329645"
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

await graphClient.Identity.B2cUserFlows["{id}"].IdentityProviders.References
    .Request()
    .UpdateAsync(identityProviders);

```